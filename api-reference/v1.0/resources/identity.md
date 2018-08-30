---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Identidade
ms.openlocfilehash: 521952ab8ea3350fcf29aa80cb82928e5017e5bb
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267161"
---
# <a name="identity-resource-type"></a><span data-ttu-id="cdf99-102">Tipo de recurso Identity</span><span class="sxs-lookup"><span data-stu-id="cdf99-102">Identity resource type</span></span>

<span data-ttu-id="cdf99-p101">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cdf99-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdf99-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdf99-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="cdf99-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdf99-106">Properties</span></span>

| <span data-ttu-id="cdf99-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdf99-107">Property</span></span>    | <span data-ttu-id="cdf99-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdf99-108">Type</span></span>   | <span data-ttu-id="cdf99-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdf99-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cdf99-110">displayName</span><span class="sxs-lookup"><span data-stu-id="cdf99-110">displayName</span></span> | <span data-ttu-id="cdf99-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdf99-111">String</span></span> | <span data-ttu-id="cdf99-p102">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem_delta.md).</span><span class="sxs-lookup"><span data-stu-id="cdf99-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem_delta.md).</span></span>     |
| <span data-ttu-id="cdf99-115">id</span><span class="sxs-lookup"><span data-stu-id="cdf99-115">id</span></span>          | <span data-ttu-id="cdf99-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdf99-116">String</span></span> | <span data-ttu-id="cdf99-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="cdf99-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a><span data-ttu-id="cdf99-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="cdf99-118">Remarks</span></span>

<span data-ttu-id="cdf99-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdf99-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->
