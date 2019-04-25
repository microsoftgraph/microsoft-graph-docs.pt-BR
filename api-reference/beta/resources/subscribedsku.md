---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda de directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582072"
---
# <a name="subscribedsku-resource-type"></a>Tipo de recurso subscribedSku

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Leia as propriedades e os relacionamentos do objeto subscribedSku.|
|[Listar subscribedsku](../api/subscribedsku-list.md) | Coleção [subscribedSku](subscribedsku.md) |Recupere a lista de assinaturas comerciais que uma organização adquiriu.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appliesTo|Cadeia de caracteres| Por exemplo, “Usuário” ou “Empresa”. |
|capabilityStatus|String| Por exemplo, "habilitado". |
|consumedUnits|Int32| O número de licenças que foram atribuídas. |
|id|String| O identificador exclusivo do objeto SKU assinado. Chave, não anulável. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Informações sobre o número e o status das licenças pré-pagas. |
|onPlans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável |
|skuId|Guid| O identificador exclusivo (GUID) do SKU do serviço. |
|skuPartNumber|Cadeia de caracteres| O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC". |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscribedsku.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
