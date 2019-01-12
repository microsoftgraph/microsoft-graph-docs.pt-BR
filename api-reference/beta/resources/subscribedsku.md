---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Expressões de filtro de consulta não são suportadas. Herda de directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01dbbf8727ab361b3763e2343e7cc72a3676848b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960151"
---
# <a name="subscribedsku-resource-type"></a>Tipo de recurso subscribedSku

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Leia as propriedades e os relacionamentos do objeto subscribedSku.|
|[Lista subscribedsku](../api/subscribedsku-list.md) | Coleção [subscribedSku](subscribedsku.md) |Recupere a lista de assinaturas comerciais que uma organização adquiriu.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appliesTo|Cadeia de caracteres| Por exemplo, “Usuário” ou “Empresa”. |
|capabilityStatus|String| Por exemplo, “Enabled”. |
|consumedUnits|Int32| O número de licenças que foram atribuídas. |
|id|Cadeia de caracteres| O identificador exclusivo do objeto SKU assinado. Chave, não anulável. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Informações sobre o número e o status das licenças pré-pagas. |
|servicePlans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável |
|skuId|Guid| O identificador exclusivo (GUID) do SKU do serviço. |
|skuPartNumber|String| O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC". |

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
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
