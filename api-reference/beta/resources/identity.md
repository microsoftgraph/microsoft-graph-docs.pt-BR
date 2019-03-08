---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
ms.openlocfilehash: 1f2d1f5a305698438748ee69f73b4143b8afd8fa
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481563"
---
# <a name="identity-resource-type"></a><span data-ttu-id="162ec-102">tipo de recurso Identity</span><span class="sxs-lookup"><span data-stu-id="162ec-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="162ec-p101">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="162ec-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="162ec-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="162ec-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="162ec-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="162ec-106">Properties</span></span>

| <span data-ttu-id="162ec-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="162ec-107">Property</span></span>            | <span data-ttu-id="162ec-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="162ec-108">Type</span></span>   | <span data-ttu-id="162ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="162ec-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="162ec-110">displayName</span><span class="sxs-lookup"><span data-stu-id="162ec-110">displayName</span></span>         | <span data-ttu-id="162ec-111">String</span><span class="sxs-lookup"><span data-stu-id="162ec-111">String</span></span> | <span data-ttu-id="162ec-p102">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="162ec-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="162ec-115">id</span><span class="sxs-lookup"><span data-stu-id="162ec-115">id</span></span>                  | <span data-ttu-id="162ec-116">String</span><span class="sxs-lookup"><span data-stu-id="162ec-116">String</span></span> | <span data-ttu-id="162ec-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="162ec-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="162ec-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="162ec-118">tenantId</span></span>            | <span data-ttu-id="162ec-119">String</span><span class="sxs-lookup"><span data-stu-id="162ec-119">String</span></span> | <span data-ttu-id="162ec-120">Identidade exclusiva do locatário (opcional).</span><span class="sxs-lookup"><span data-stu-id="162ec-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="162ec-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="162ec-121">Remarks</span></span>

<span data-ttu-id="162ec-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="162ec-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

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
