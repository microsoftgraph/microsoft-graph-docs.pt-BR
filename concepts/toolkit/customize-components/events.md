---
title: Manipular eventos expostos pelos componentes Graph Toolkit Microsoft
description: Muitos componentes Graph Toolkit Microsoft emitem eventos personalizados. Anexar manipuladores de eventos a esses eventos permite que você responda a eles e controle o comportamento do seu aplicativo.
ms.localizationpriority: medium
author: waldekmastykarz
ms.openlocfilehash: 31dacb14c4b4faacc7f97626fef0977bbf74b443
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890588"
---
# <a name="handle-events-exposed-by-microsoft-graph-toolkit-components"></a>Manipular eventos expostos pelos componentes Graph Toolkit Microsoft

Muitos componentes Graph Toolkit Microsoft emitem eventos personalizados. Anexar manipuladores de eventos a esses eventos permite que você responda a eles e controle o comportamento do seu aplicativo.

## <a name="discover-which-events-components-emit"></a>Descobrir quais componentes de eventos emitem

Cada componente Graph Toolkit Microsoft emite eventos diferentes, específicos de sua funcionalidade. Para ver a lista de eventos emitidos pelo componente específico, consulte a seção **Eventos** da documentação desse componente.

> [!IMPORTANT]
> Alguns eventos, como `itemClick` no componente de lista de arquivos, são emitidos somente ao usar o modelo padrão. Se você usar um modelo personalizado, sobrescreve a renderização padrão responsável pela emissão do evento.

## <a name="add-event-handlers-to-events"></a>Adicionar manipuladores de eventos a eventos

A Microsoft Graph Toolkit usa a [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) função padrão para emitir eventos personalizados em seus componentes. Para anexar um manipulador de eventos a um evento personalizado emitido pelo componente de um kit de ferramentas, use a função [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) padrão.

Por exemplo, para manipular o evento emitido pelo componente de lista `itemClick` arquivo, adicione o seguinte ao código.

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  // your event handler code goes here
});
```

### <a name="access-additional-information-exposed-by-the-event"></a>Acessar informações adicionais expostas pelo evento

Alguns eventos emitidos pela Microsoft Graph Toolkit contêm informações adicionais relevantes para o evento. Por exemplo, o evento, emitido pelo componente de lista Arquivo, contém informações sobre o arquivo que foi clicado `itemClick` na lista de arquivos. Para ver se o evento específico contém informações adicionais, consulte a seção **Eventos** da documentação do componente correspondente.

Você pode acessar as informações adicionais expostas por um evento por meio da propriedade do objeto passado para o manipulador de eventos, conforme `details` mostrado no exemplo a `event` seguir.

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  const clickedFile = e.details;
});
```
