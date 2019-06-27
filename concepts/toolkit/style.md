---
title: Estilizando o Microsoft Graph Toolkit
description: Usar propriedades personalizadas de CSS para modificar os estilos de componente
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 41262c4e58973d84f4fec56a6d5abe8dfaf555ef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242932"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Estilos de componentes no Microsoft Graph Toolkit

Use Propriedades personalizadas de CSS para modificar os estilos de componente.

Cada componente documenta um conjunto de [Propriedades personalizadas de CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) que você pode usar para alterar a aparência de determinados elementos. Por exemplo:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Você não pode estilizar elementos internos de um componente, a menos que forneça uma propriedade personalizada de CSS. Os elementos filho do componente estão hospedados em um [dom de sombra](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).

Para obter mais flexibilidade, considere o uso de [modelos personalizados](./templates.md).

## <a name="disable-the-shadow-dom-experimental"></a>Desabilitar o dom de sombra (experimental)

Você pode desabilitar o dom de sombra e estilizar diretamente elementos internos usando folhas de estilo normais do navegador, definindo a `useShadowDom` propriedade estática `MgtBaseComponent` da classe como false antes de usar qualquer marca de gerenciamento.


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
