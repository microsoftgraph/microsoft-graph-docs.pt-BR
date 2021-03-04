---
title: Tipo de recurso userSource
description: O contêiner para a caixa de correio de um custodiado e o site do OneDrive for Business.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445941"
---
# <a name="usersource-resource-type"></a>Tipo de recurso userSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner para a [caixa de correio de um custodiado](ediscovery-custodian.md) e o site do OneDrive for Business.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userSources](../api/ediscovery-custodian-list-usersources.md)|[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Obter uma lista dos **objetos userSource** e suas propriedades.|
|[Criar userSource](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Crie um novo **objeto userSource.**|
|[Obter userSource](../api/ediscovery-usersource-get.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Leia as propriedades e as relações de um **objeto userSource.**|
|[Excluir userSource](../api/ediscovery-usersource-delete.md)|Nenhum(a)|**Exclua um objeto userSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o userSource**.|
|createdDateTime|DateTimeOffset|A data e a hora **em que o userSource** foi criado|
|displayName|String|O nome de exibição associado à caixa de correio e ao site.|
|email|Cadeia de caracteres|Endereço de email da caixa de correio do usuário.|
|id|String|A ID do **userSource**. Essa não é a ID do grupo real|
|includedSources|microsoft.graph.ediscovery.sourceType|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|

### <a name="sourcetype-values"></a>valores sourceType

Tipos de fonte relacionados ao usuário. Inclui caixa de correio e site por padrão.

|Member|Descrição|
|:----|-----------|
|mailbox|Representa uma caixa de correio.|
|site|Representa um site do OneDrive for Business.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```
