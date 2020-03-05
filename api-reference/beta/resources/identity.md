---
author: JeremyKelley
description: O recurso Identity representa uma identidade de um actor.
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ebfc032008bf478c3c66883aceb802992704f46d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496800"
---
# <a name="identity-resource-type"></a><span data-ttu-id="053d8-103">tipo de recurso Identity</span><span class="sxs-lookup"><span data-stu-id="053d8-103">identity resource type</span></span>

<span data-ttu-id="053d8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="053d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="053d8-p101">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="053d8-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="053d8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="053d8-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="053d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="053d8-108">Properties</span></span>

| <span data-ttu-id="053d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="053d8-109">Property</span></span>            | <span data-ttu-id="053d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="053d8-110">Type</span></span>   | <span data-ttu-id="053d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="053d8-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="053d8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="053d8-112">displayName</span></span>         | <span data-ttu-id="053d8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="053d8-113">String</span></span> | <span data-ttu-id="053d8-p102">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="053d8-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="053d8-117">id</span><span class="sxs-lookup"><span data-stu-id="053d8-117">id</span></span>                  | <span data-ttu-id="053d8-118">String</span><span class="sxs-lookup"><span data-stu-id="053d8-118">String</span></span> | <span data-ttu-id="053d8-119">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="053d8-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="053d8-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="053d8-120">tenantId</span></span>            | <span data-ttu-id="053d8-121">String</span><span class="sxs-lookup"><span data-stu-id="053d8-121">String</span></span> | <span data-ttu-id="053d8-122">Identidade exclusiva do locatário (opcional).</span><span class="sxs-lookup"><span data-stu-id="053d8-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="053d8-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="053d8-123">Remarks</span></span>

<span data-ttu-id="053d8-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="053d8-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->
