---
title: Tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
ms.openlocfilehash: 1f0992904a124931be239fd18ad2bf187e01c41c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885747"
---
# <a name="licensedetails-resource-type"></a>Tipo de recurso licenseDetails

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém informações sobre uma licença atribuída a um usuário.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar licenseDetails](../api/user-list-licensedetails.md) | coleção licenseDetails |Recupere uma lista de objetos licenseDetails para um usuário.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| O identificador exclusivo do objeto de detalhe de licença. Somente leitura, Chave, Não anulável |
|servicePlans|Coleção [servicePlanInfo](serviceplaninfo.md)| Informações sobre os planos de serviços que estão disponíveis com a licença. Somente leitura, Não anulável |
|skuId|Guid| O identificador exclusivo (GUID) do SKU do serviço. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura |
|skuPartNumber|String| Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura |

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
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
