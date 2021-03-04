---
title: Tipo de recurso siteSource
description: O contêiner de um site associado a um custodiado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa4b8d0ccbe80ef0f65d27fa8ef648d1ea07b63
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445896"
---
# <a name="sitesource-resource-type"></a>Tipo de recurso siteSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner de um site associado a um [custodiado](ediscovery-custodian.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar siteSources](../api/ediscovery-custodian-list-sitesources.md)|[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Obter uma lista de **objetos siteSource** e suas propriedades.|
|[Criar siteSource](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Crie um novo **objeto siteSource.**|
|[Obter siteSource](../api/ediscovery-sitesource-get.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Leia as propriedades e as relações de um **objeto siteSource.**|
|[Excluir siteSource](../api/ediscovery-sitesource-delete.md)|Nenhum(a)|Excluir um **objeto siteSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o siteSource**.|
|createdDateTime|DateTimeOffset|A data e a hora **em que o siteSource** foi criado.|
|displayName|String|O nome de exibição **do siteSource**. Esse será o nome do site do SharePoint.|
|id|String| A ID do **siteSource**. Essa não é a ID do site real.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|site|[site](../resources/site.md)|O site do SharePoint associado ao **siteSource**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
