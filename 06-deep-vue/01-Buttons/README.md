# Buttons

Требуется разработать компоненты кнопок.

Основным компонентом будет `BaseButton`:
- Входные параметры:
    - `block` - логический, является ли кнопка блоком (с классом `button_block`);
    - `tag` - строковый параметр, элемент, который используется для кнопки (`button`, `a`, `router-link`), по умолчанию `button`. Именно над этим элементом компонент должен быть прозрачной обёрткой. Это удобно, так как часто визуально кнопка может вести себя как кнопка, а может, как ссылка;
- Слот по умолчанию - содержимое кнопки;
- Параметр `tag` должен проверяться валидатором на допустимые значения;
- На кнопке должны работать все стандартные события (такие, как `click`) без добавления модификатора `.native`.

Ещё три кнопки основаны на `BaseButton` и являются обёртками над ним:
- `PrimaryButton` - это `BaseButton` с классом `button_primary`;
- `SecondaryButton` - это `BaseButton` с классом `button_secondary`;
- `DangerButton` - это `BaseButton` с классом `button_danger`.

---

### Инструкция

📝 Для решения задачи отредактируйте файлы: `components/BaseButton.vue`, `components/PrimaryButton.vue`, `components/SecondaryButton.vue`, `components/DangerButton.vue`.

🚀 Команда запуска для ручного тестирования: `npm run serve`;<br>
приложение будет доступно на [http://localhost:8080/06-deep-vue/01-Buttons](http://localhost:8080/06-deep-vue/01-Buttons).

✅ Доступно автоматическое тестирование: `npm test Buttons`.
