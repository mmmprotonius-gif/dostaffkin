# dostaffkin

Приложение для расчёта доставки и отслеживания отправлений.

## Что делает
- Страница заказа рассчитывает маршрут между адресами через Yandex Maps.
- Подбирает стоимость по размеру посылки и скорости доставки.
- Отправляет заявку на API `https://testologia.ru/delivery/create`.
- Страница трекинга запрашивает статус отправления по номеру через `https://testologia.ru/delivery/info`.

## Структура
- `src/app/pages/order` — форма заказа и карта маршрута.
- `src/app/pages/track` — поиск статуса по номеру отправления.
- `src/app/services/delivery-api.ts` — HTTP-клиент для внешнего API.
- `src/app/app.routes.ts` — маршруты: `/`, `/order`, `/track`.

## Стек
- Angular 21
- TypeScript
- RxJS
- ngx-toastr
- Yandex Maps API (в браузере)

## Запуск
```bash
npm install
npm start
```

## Сборка
```bash
npm run build
```

## Тесты
```bash
npm test
```
