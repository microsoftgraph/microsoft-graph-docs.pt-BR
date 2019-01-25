---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
ms.openlocfilehash: 1ac2aea59ab0d6b09ae613b72fbfbf924240a4a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518790"
---
# <a name="identity-resource-type"></a><span data-ttu-id="98db2-102">tipo de recurso de identidade</span><span class="sxs-lookup"><span data-stu-id="98db2-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98db2-p101">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98db2-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98db2-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98db2-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="98db2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98db2-106">Properties</span></span>

| <span data-ttu-id="98db2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98db2-107">Property</span></span>            | <span data-ttu-id="98db2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="98db2-108">Type</span></span>   | <span data-ttu-id="98db2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="98db2-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="98db2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="98db2-110">displayName</span></span>         | <span data-ttu-id="98db2-111">String</span><span class="sxs-lookup"><span data-stu-id="98db2-111">String</span></span> | <span data-ttu-id="98db2-p102">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="98db2-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="98db2-115">id</span><span class="sxs-lookup"><span data-stu-id="98db2-115">id</span></span>                  | <span data-ttu-id="98db2-116">String</span><span class="sxs-lookup"><span data-stu-id="98db2-116">String</span></span> | <span data-ttu-id="98db2-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="98db2-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="98db2-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="98db2-118">tenantId</span></span>            | <span data-ttu-id="98db2-119">String</span><span class="sxs-lookup"><span data-stu-id="98db2-119">String</span></span> | <span data-ttu-id="98db2-120">Identidade exclusiva do inquilino (opcional).</span><span class="sxs-lookup"><span data-stu-id="98db2-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="98db2-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="98db2-121">Remarks</span></span>

<span data-ttu-id="98db2-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="98db2-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": [
    "Error: /api-reference/beta/resources/identity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
