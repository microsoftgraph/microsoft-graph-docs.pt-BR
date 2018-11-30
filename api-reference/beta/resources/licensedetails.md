---
title: Tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
ms.openlocfilehash: dd56026d2c1d230fe6bb25b78ff8ababa01f577b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040725"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="6160f-103">Tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="6160f-103">licenseDetails resource type</span></span>

> <span data-ttu-id="6160f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6160f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6160f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6160f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6160f-106">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="6160f-106">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="6160f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6160f-107">Methods</span></span>

| <span data-ttu-id="6160f-108">Método</span><span class="sxs-lookup"><span data-stu-id="6160f-108">Method</span></span>           | <span data-ttu-id="6160f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6160f-109">Return Type</span></span>    |<span data-ttu-id="6160f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6160f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6160f-111">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="6160f-111">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="6160f-112">coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="6160f-112">licenseDetails collection</span></span> |<span data-ttu-id="6160f-113">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="6160f-113">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="6160f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6160f-114">Properties</span></span>
| <span data-ttu-id="6160f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6160f-115">Property</span></span>     | <span data-ttu-id="6160f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="6160f-116">Type</span></span>   |<span data-ttu-id="6160f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6160f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6160f-118">id</span><span class="sxs-lookup"><span data-stu-id="6160f-118">id</span></span>|<span data-ttu-id="6160f-119">String</span><span class="sxs-lookup"><span data-stu-id="6160f-119">String</span></span>| <span data-ttu-id="6160f-p102">O identificador exclusivo do objeto de detalhe de licença. Somente leitura, Chave, Não anulável</span><span class="sxs-lookup"><span data-stu-id="6160f-p102">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="6160f-122">servicePlans</span><span class="sxs-lookup"><span data-stu-id="6160f-122">servicePlans</span></span>|<span data-ttu-id="6160f-123">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="6160f-123">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="6160f-p103">Informações sobre os planos de serviços que estão disponíveis com a licença. Somente leitura, Não anulável</span><span class="sxs-lookup"><span data-stu-id="6160f-p103">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="6160f-126">skuId</span><span class="sxs-lookup"><span data-stu-id="6160f-126">skuId</span></span>|<span data-ttu-id="6160f-127">Guid</span><span class="sxs-lookup"><span data-stu-id="6160f-127">Guid</span></span>| <span data-ttu-id="6160f-p104">O identificador exclusivo (GUID) do SKU do serviço. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="6160f-p104">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="6160f-131">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="6160f-131">skuPartNumber</span></span>|<span data-ttu-id="6160f-132">String</span><span class="sxs-lookup"><span data-stu-id="6160f-132">String</span></span>| <span data-ttu-id="6160f-p105">Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura</span><span class="sxs-lookup"><span data-stu-id="6160f-p105">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="6160f-136">Relações</span><span class="sxs-lookup"><span data-stu-id="6160f-136">Relationships</span></span>
<span data-ttu-id="6160f-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6160f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6160f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6160f-138">JSON representation</span></span>
<span data-ttu-id="6160f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6160f-139">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->