---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
ms.localizationpriority: medium
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: dd497dd40e691fe8751517b7c9b540844e29e615
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134451"
---
# <a name="subscribedsku-resource-type"></a>Tipo de recurso subscribedSku

Namespace: microsoft.graph

Contém informações sobre um serviço SKU assinado por uma empresa.

Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Obter uma assinatura comercial específica que uma organização adquiriu.|
|[Listar subscribedsku](../api/subscribedsku-list.md) | Coleção [subscribedSku](subscribedsku.md) |Obtenha a lista de assinaturas comerciais que uma organização adquiriu.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appliesTo|Cadeia de caracteres| Por exemplo, “Usuário” ou “Empresa”. |
|capabilityStatus|Cadeia de caracteres|  Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`. O capabilityStatus é se a propriedade `Enabled` **prepaidUnits** tiver pelo menos uma unidade habilitada e se o cliente `LockedOut` cancelar sua assinatura. |
|consumedUnits|Int32| O número de licenças que foram atribuídas. |
|id|Cadeia de caracteres| O identificador exclusivo do objeto SKU assinado. Chave, não anulada. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Informações sobre o número e o status das licenças pré-pagas. |
|servicePlans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulada |
|skuId|Guid| O identificador exclusivo (GUID) do SKU do serviço. |
|skuPartNumber|Cadeia de caracteres| O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC". Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [List subscribedSkus](../api/subscribedsku-list.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```

## <a name="see-also"></a>Confira também

+ [Nomes de produtos e identificadores de plano de serviço para licenciamento](/azure/active-directory/enterprise-users/licensing-service-plan-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

