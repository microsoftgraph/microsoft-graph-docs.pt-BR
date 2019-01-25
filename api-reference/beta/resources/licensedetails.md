---
title: Tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
ms.openlocfilehash: 7036904e20173f8fefb6f4f02bd2473289de96c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522774"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="0659c-103">Tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="0659c-103">licenseDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0659c-104">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="0659c-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="0659c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0659c-105">Methods</span></span>

| <span data-ttu-id="0659c-106">Método</span><span class="sxs-lookup"><span data-stu-id="0659c-106">Method</span></span>           | <span data-ttu-id="0659c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0659c-107">Return Type</span></span>    |<span data-ttu-id="0659c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0659c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0659c-109">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="0659c-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="0659c-110">coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="0659c-110">licenseDetails collection</span></span> |<span data-ttu-id="0659c-111">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="0659c-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="0659c-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0659c-112">Properties</span></span>
| <span data-ttu-id="0659c-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0659c-113">Property</span></span>     | <span data-ttu-id="0659c-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="0659c-114">Type</span></span>   |<span data-ttu-id="0659c-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0659c-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0659c-116">id</span><span class="sxs-lookup"><span data-stu-id="0659c-116">id</span></span>|<span data-ttu-id="0659c-117">String</span><span class="sxs-lookup"><span data-stu-id="0659c-117">String</span></span>| <span data-ttu-id="0659c-p101">O identificador exclusivo do objeto de detalhe de licença. Somente leitura, Chave, Não anulável</span><span class="sxs-lookup"><span data-stu-id="0659c-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="0659c-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="0659c-120">servicePlans</span></span>|<span data-ttu-id="0659c-121">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="0659c-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="0659c-p102">Informações sobre os planos de serviços que estão disponíveis com a licença. Somente leitura, Não anulável</span><span class="sxs-lookup"><span data-stu-id="0659c-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="0659c-124">skuId</span><span class="sxs-lookup"><span data-stu-id="0659c-124">skuId</span></span>|<span data-ttu-id="0659c-125">Guid</span><span class="sxs-lookup"><span data-stu-id="0659c-125">Guid</span></span>| <span data-ttu-id="0659c-p103">O identificador exclusivo (GUID) do SKU do serviço. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0659c-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="0659c-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="0659c-129">skuPartNumber</span></span>|<span data-ttu-id="0659c-130">String</span><span class="sxs-lookup"><span data-stu-id="0659c-130">String</span></span>| <span data-ttu-id="0659c-p104">Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0659c-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="0659c-134">Relações</span><span class="sxs-lookup"><span data-stu-id="0659c-134">Relationships</span></span>
<span data-ttu-id="0659c-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0659c-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0659c-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0659c-136">JSON representation</span></span>
<span data-ttu-id="0659c-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0659c-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licensedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
