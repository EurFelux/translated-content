---
title: Способ разметки
slug: Glossary/Layout_mode
---

{{CSSRef}}

[CSS](/ru/docs/Web/CSS) **способ разметки** (или _раскладки,_ или англ. _layout_) — это алгоритм определения позиции и размеров блоков, основанный на способе, которым они взаимодействуют с родственными блоками. Существует несколько типов разметки:

- _Обычная (Normal Flow)_ — все элементы являются частью обычного потока до тех пор, пока вы не переопределите это каким-либо образом. Обычный _layout_ включает в себя _блочную раскладку_, созданную для расположения отдельных блоков, таких как параграфы, и _линейную_, — для строчных элементов;
- _[Табличная](/ru/docs/Web/CSS/CSS_table)_, спроектированная для расположения таблиц;
- _Float layout_ — для возможности обозначить элементы _[плавающими](/ru/docs/Web/CSS/float)._ Такой элемент начинает позиционироваться слева или справа относительно содержимого обычного потока, элементы которого начинают обтекать него;
- _[Позиционированная](/ru/docs/Web/CSS/CSS_positioned_layout) _— для позиционирования элементов без особого взаимодействия с другими элементами;
- _[Множественные столбцы](/ru/docs/Web/CSS/CSS_multicol_layout)_ — для расположения контента колонками, как в газетах;
- _[Флексбокс](/ru/docs/Web/CSS/CSS_flexible_box_layout) (CSS Flexible Box Layout)_ — для расположения сложных страниц, которые плавно могут изменять свой размер; {{ experimental_inline() }}
- _[Сеточная](/ru/docs/Web/CSS/CSS_grid_layout)_ — для расположения элементов относительно фиксированной сетки. {{ experimental_inline() }}

> [!NOTE]
> Не все [CSS-свойства](/ru/docs/Web/CSS/Reference) применимы ко всем способам разметки. Большинство из них применяются к одному или двум из них и не действуют, если применяются на элементе, участвующем в другом режиме разметки.

## Смотрите также

- Ключевые концепции CSS
  - [Синтаксис CSS](/ru/docs/Web/CSS/CSS_syntax/Syntax)
  - [@-правила](/ru/docs/Web/CSS/CSS_syntax/At-rule)
  - [комментарии](/ru/docs/Web/CSS/CSS_syntax/Comments)
  - [специфичность](/ru/docs/Web/CSS/CSS_cascade/Specificity)
  - [наследование](/ru/docs/Web/CSS/CSS_cascade/Inheritance)
  - [блочная модель](/ru/docs/Web/CSS/CSS_box_model/Introduction_to_the_CSS_box_model)
  - [режимы компоновки](/ru/docs/Glossary/Layout_mode)
  - [модели визуального форматирования](/ru/docs/Web/CSS/CSS_display/Visual_formatting_model)
  - [Схлопывание отступов](/ru/docs/Web/CSS/CSS_box_model/Mastering_margin_collapsing)
  - Значения
    - [начальные](/ru/docs/conflicting/Web/CSS/CSS_cascade/Value_processing)
    - [вычисленные](/ru/docs/conflicting/Web/CSS/CSS_cascade/Value_processing_e3410028f0a698ddd9f74225ea8d122c0a582707d683fdd173e681e62003518d)
    - [используемые](/ru/docs/conflicting/Web/CSS/CSS_cascade/Value_processing_67ecc2d1089286b6003d201c901ee7218b8f627858ae89823dc40509095cd65b)
    - [действительные](/ru/docs/Web/CSS/CSS_cascade/Value_processing)
  - [Синтаксис определения значений](/ru/docs/Web/CSS/Value_definition_syntax)
  - [Сокращённые свойства](/ru/docs/Web/CSS/CSS_cascade/Shorthand_properties)
  - [Замещаемые элементы](/ru/docs/Web/CSS/CSS_images/Replaced_element_properties)
