# Задание 2: Проектирование API

## 1. Пример REST API запроса

Так как этот экран ответственен за отображение информации о **магазинах** партнеров, эндпоинт предлагаю назвать следующим образом:

**GET /petrushka/stores**

**Заголовки запроса:**

| Заголовок | Описание | Тип |
|-----------|----------|-----|
| Authorization | Токен авторизации пользователя в формате Bearer. Необходим для идентификации пользователя и контроля доступа | String |
| Accept | Формат ответа, который ожидает клиент: application/json | String |

## 2. Пример ответа REST API

```json
{
  "status": "success",
  "data": {
    "stores": [
      {
        "id": "metro_001",
        "name": "METRO",
        "logo_url": "https://cdn.petrushka.ru/partners/logos/metro.png",
        "delivery_info": "Ближайшая доставка сегодня 21:00–23:00",
        "external_url": "https://metro.ru/petrushka/partner"
      },
      {
        "id": "ashan_002",
        "name": "Ашан",
        "logo_url": "https://cdn.petrushka.ru/partners/logos/ashan.png",
        "delivery_info": "Ближайшая доставка сегодня 18:00–20:00",
        "external_url": "https://ashan.ru/petrushka/partner"
      },
      {
        "id": "vkusvill_003",
        "name": "ВкусВилл",
        "logo_url": "https://cdn.petrushka.ru/partners/logos/vkusvill.png",
        "delivery_info": "Быстрая доставка от 20 до 60 минут",
        "external_url": "https://vkusvill.ru/petrushka/partner"
      },
      {
        "id": "victoria_004",
        "name": "ВИКТОРИЯ",
        "logo_url": "https://cdn.petrushka.ru/partners/logos/victoria.png",
        "delivery_info": "Ближайшая доставка сегодня 17:00–19:00",
        "external_url": "https://victoria.ru/petrushka/partner"
      }
    ]
  }
}
