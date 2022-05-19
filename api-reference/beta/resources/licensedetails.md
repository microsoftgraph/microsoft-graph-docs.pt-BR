---
title: Tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jconley76
ms.openlocfilehash: 220c164e4acf119a7937e4ab5674b93fb7a64af0
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549502"
---
# <a name="licensedetails-resource-type"></a>Tipo de recurso licenseDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre uma licença atribuída a um usuário.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar licenseDetails](../api/user-list-licensedetails.md) | Coleção licenseDetails |Recupere uma lista de objetos licenseDetails para um usuário.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| O identificador exclusivo do objeto de detalhes da licença. Somente leitura, chave, não anulável |
|servicePlans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos de serviço atribuídos com a licença. Somente leitura, não anulável |
|skuId|Guid| Identificador exclusivo (GUID) para o SKU de serviço. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura |
|skuPartNumber|Cadeia de caracteres| Nome de exibição de SKU exclusivo. Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium". Somente leitura |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

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
  "suppressions": []
}
-->


