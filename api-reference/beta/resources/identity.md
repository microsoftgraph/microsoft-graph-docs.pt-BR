---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
ms.openlocfilehash: a2ba76d5bac372be0a40001028dfb54e690a14fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333664"
---
# <a name="identity-resource-type"></a><span data-ttu-id="4aad5-102">tipo de recurso Identity</span><span class="sxs-lookup"><span data-stu-id="4aad5-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aad5-p101">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4aad5-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4aad5-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4aad5-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="4aad5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4aad5-106">Properties</span></span>

| <span data-ttu-id="4aad5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4aad5-107">Property</span></span>            | <span data-ttu-id="4aad5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4aad5-108">Type</span></span>   | <span data-ttu-id="4aad5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aad5-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4aad5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4aad5-110">displayName</span></span>         | <span data-ttu-id="4aad5-111">String</span><span class="sxs-lookup"><span data-stu-id="4aad5-111">String</span></span> | <span data-ttu-id="4aad5-p102">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="4aad5-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="4aad5-115">id</span><span class="sxs-lookup"><span data-stu-id="4aad5-115">id</span></span>                  | <span data-ttu-id="4aad5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4aad5-116">String</span></span> | <span data-ttu-id="4aad5-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="4aad5-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="4aad5-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="4aad5-118">tenantId</span></span>            | <span data-ttu-id="4aad5-119">String</span><span class="sxs-lookup"><span data-stu-id="4aad5-119">String</span></span> | <span data-ttu-id="4aad5-120">Identidade exclusiva do locatário (opcional).</span><span class="sxs-lookup"><span data-stu-id="4aad5-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="4aad5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="4aad5-121">Remarks</span></span>

<span data-ttu-id="4aad5-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="4aad5-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

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
