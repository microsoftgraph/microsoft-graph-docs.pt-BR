---
title: tipo de recurso username
description: O contêiner para a caixa de correio de um dos responsáveis e o site do OneDrive for Business.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597482"
---
# <a name="usersource-resource-type"></a>tipo de recurso username

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner para a caixa de correio de um dos responsáveis e o site [do](custodian.md) onedrive for Business.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usersources](../api/custodian-list-usersources.md)|coleção [username](../resources/usersource.md)|Obtenha uma lista dos objetos **username** e suas propriedades.|
|[Criar usuário](../api/custodian-post-usersources.md)|[username](../resources/usersource.md)|Criar um novo objeto **username** .|
|[Obter usuário](../api/usersource-get.md)|[username](../resources/usersource.md)|Leia as propriedades e os relacionamentos de um objeto **username** .|
|[Excluir usuário](../api/usersource-delete.md)|Nenhum|Excluir um objeto **username** .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a **username**.|
|createdDateTime|DateTimeOffset|A data e a hora em que o **usuário** da erSource foi criado|
|displayName|String|O nome de exibição associado à caixa de correio e ao site.|
|email|Cadeia de caracteres|Endereço de email da caixa de correio do usuário.|
|id|String|A ID da **username**. Essa não é a ID do grupo real|
|includedSources|sourceType|Especifica quais fontes são incluídas nesse grupo. Os valores possíveis são: `mailbox` e `site`.|

### <a name="sourcetype-values"></a>valores de sourceType

Tipos de fonte relacionados ao usuário. Inclui a caixa de correio e o site por padrão.

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
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
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
