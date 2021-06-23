---
title: Manipular eventos expostos pelos componentes Graph Toolkit Microsoft
description: Muitos componentes Graph Toolkit Microsoft emitem eventos personalizados. Anexar manipuladores de eventos a esses eventos permite que você responda a eles e controle o comportamento do seu aplicativo.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: f20de269ed7f304f9c1d7198475b6fdb81b709c7
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082388"
---
# <a name="handle-events-exposed-by-microsoft-graph-toolkit-components"></a><span data-ttu-id="66bd7-104">Manipular eventos expostos pelos componentes Graph Toolkit Microsoft</span><span class="sxs-lookup"><span data-stu-id="66bd7-104">Handle events exposed by Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="66bd7-105">Muitos componentes Graph Toolkit Microsoft emitem eventos personalizados.</span><span class="sxs-lookup"><span data-stu-id="66bd7-105">Many Microsoft Graph Toolkit components emit custom events.</span></span> <span data-ttu-id="66bd7-106">Anexar manipuladores de eventos a esses eventos permite que você responda a eles e controle o comportamento do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66bd7-106">Attaching event handlers to these events allows you to respond to them and control the behavior of your app.</span></span>

## <a name="discover-which-events-components-emit"></a><span data-ttu-id="66bd7-107">Descobrir quais componentes de eventos emitem</span><span class="sxs-lookup"><span data-stu-id="66bd7-107">Discover which events components emit</span></span>

<span data-ttu-id="66bd7-108">Cada componente Graph Toolkit Microsoft emite eventos diferentes, específicos de sua funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="66bd7-108">Each Microsoft Graph Toolkit component emits different events, specific to its functionality.</span></span> <span data-ttu-id="66bd7-109">Para ver a lista de eventos emitidos pelo componente específico, consulte a seção **Eventos** da documentação desse componente.</span><span class="sxs-lookup"><span data-stu-id="66bd7-109">To see the list of events emitted by the specific component, see the **Events** section of the documentation for that component.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="66bd7-110">Alguns eventos, como `itemClick` no componente de lista de arquivos, são emitidos somente ao usar o modelo padrão.</span><span class="sxs-lookup"><span data-stu-id="66bd7-110">Some events, like `itemClick` in the File list component, are emitted only when using the default template.</span></span> <span data-ttu-id="66bd7-111">Se você usar um modelo personalizado, sobrescreve a renderização padrão responsável pela emissão do evento.</span><span class="sxs-lookup"><span data-stu-id="66bd7-111">If you use a custom template, you overwrite the default rendering that is responsible for emitting the event.</span></span>

## <a name="add-event-handlers-to-events"></a><span data-ttu-id="66bd7-112">Adicionar manipuladores de eventos a eventos</span><span class="sxs-lookup"><span data-stu-id="66bd7-112">Add event handlers to events</span></span>

<span data-ttu-id="66bd7-113">A Microsoft Graph Toolkit usa a [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) função padrão para emitir eventos personalizados em seus componentes.</span><span class="sxs-lookup"><span data-stu-id="66bd7-113">Microsoft Graph Toolkit uses the standard [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) function to emit custom events in its components.</span></span> <span data-ttu-id="66bd7-114">Para anexar um manipulador de eventos a um evento personalizado emitido pelo componente de um kit de ferramentas, use a função [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) padrão.</span><span class="sxs-lookup"><span data-stu-id="66bd7-114">To attach an event handler to a custom event emitted by a toolkit's component, use the standard [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) function.</span></span>

<span data-ttu-id="66bd7-115">Por exemplo, para manipular o evento emitido pelo componente de lista `itemClick` arquivo, adicione o seguinte ao código.</span><span class="sxs-lookup"><span data-stu-id="66bd7-115">For example, to handle the `itemClick` event emitted by the File list component, add the following to your code.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick' e => {
  // your event handler code goes here
});
```

### <a name="access-additional-information-exposed-by-the-event"></a><span data-ttu-id="66bd7-116">Acessar informações adicionais expostas pelo evento</span><span class="sxs-lookup"><span data-stu-id="66bd7-116">Access additional information exposed by the event</span></span>

<span data-ttu-id="66bd7-117">Alguns eventos emitidos pela Microsoft Graph Toolkit contêm informações adicionais relevantes para o evento.</span><span class="sxs-lookup"><span data-stu-id="66bd7-117">Some events emitted by Microsoft Graph Toolkit contain additional information relevant to the event.</span></span> <span data-ttu-id="66bd7-118">Por exemplo, o evento, emitido pelo componente de lista Arquivo, contém informações sobre o arquivo que foi clicado `itemClick` na lista de arquivos.</span><span class="sxs-lookup"><span data-stu-id="66bd7-118">For example, the `itemClick` event, emitted by the File list component, contains information about the file that was clicked in the file list.</span></span> <span data-ttu-id="66bd7-119">Para ver se o evento específico contém informações adicionais, consulte a seção **Eventos** da documentação do componente correspondente.</span><span class="sxs-lookup"><span data-stu-id="66bd7-119">To see if the particular event contains additional information, see the **Events** section of the documentation for the corresponding component.</span></span>

<span data-ttu-id="66bd7-120">Você pode acessar as informações adicionais expostas por um evento por meio da propriedade do objeto passado para o manipulador de eventos, conforme `details` mostrado no exemplo a `event` seguir.</span><span class="sxs-lookup"><span data-stu-id="66bd7-120">You can access the additional information exposed by an event through the `details` property of the `event` object passed into your event handler, as shown in the following example.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  const clickedFile = e.details;
});
```
