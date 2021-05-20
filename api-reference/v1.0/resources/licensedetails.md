---
title: licenciamentoDeseto de recurso
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4e23dfcd15dc2b05a9d1c7356a532e6faf487662
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547187"
---
# <a name="licensedetails-resource-type"></a>licenciamentoDeseto de recurso

Namespace: microsoft.graph

Contém informações sobre uma licença atribuída a um usuário.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar licenseDetails](../api/user-list-licensedetails.md) | Coleção licenseDetails |Recuperar uma lista de objetos de licençade detalhes para um usuário.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| O identificador exclusivo para o objeto de detalhe de licença. Somente leitura, chave, não é nulo |
|planos de serviço|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos de serviço atribuídos à licença. Somente leitura, não é nulo |
|skuId|Guid| Identificador exclusivo (GUID) para o serviço SKU. Igual à propriedade skuId no objeto [AssinadSku](subscribedsku.md) relacionado. Somente leitura |
|skuPartNumber|Cadeia de caracteres| Nome de exibição SKU exclusivo. Igual ao skuPartNumber no objeto [AssinadSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium". Somente leitura |

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

