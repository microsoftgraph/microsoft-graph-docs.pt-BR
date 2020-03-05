---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d6f5824823af71f5ce7c1a63dce9d73eca8e5c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447588"
---
# <a name="licensedetails-resource-type"></a>tipo de recurso licenseDetails

Namespace: Microsoft. Graph

Contém informações sobre uma licença atribuída a um usuário.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar licenseDetails](../api/user-list-licensedetails.md) | Coleção licenseDetails |Recupere uma lista de objetos licenseDetails para um usuário.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| O identificador exclusivo do objeto de detalhes da licença. Somente leitura, chave, não anulável |
|onplans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos de serviço atribuídos com a licença. Somente leitura, não nulo |
|skuId|Guid| Identificador exclusivo (GUID) do serviço SKU. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura |
|skuPartNumber|Cadeia de caracteres| Nome de exibição SKU exclusivo. Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium". Somente leitura |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
