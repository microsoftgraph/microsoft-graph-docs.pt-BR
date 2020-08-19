---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5c71c870d8b078a47acc4a0a0f968bcdedb760f2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812804"
---
# <a name="licensedetails-resource-type"></a>tipo de recurso licenseDetails

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
