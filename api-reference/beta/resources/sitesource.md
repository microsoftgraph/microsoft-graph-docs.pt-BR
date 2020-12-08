---
title: tipo de recurso de site da filial
description: O contêiner de um site associado a um responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597529"
---
# <a name="sitesource-resource-type"></a>tipo de recurso de site da filial

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner de um site associado a um [responsáveis](custodian.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar siteSources](../api/custodian-list-sitesources.md)|coleção de [sites de site](../resources/sitesource.md)|Obter uma lista de objetos de **site de site** e suas propriedades.|
|[Criar site local](../api/custodian-post-sitesources.md)|[site da site](../resources/sitesource.md)|Criar um novo objeto **sitery** .|
|[Obter local de site](../api/sitesource-get.md)|[site da site](../resources/sitesource.md)|Leia as propriedades e os relacionamentos de um objeto de **site** .|
|[Excluir site local](../api/sitesource-delete.md)|Nenhum|Excluir um objeto de **site** .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a **site**.|
|createdDateTime|DateTimeOffset|A data e a hora em que o **site local** foi criado.|
|displayName|String|O nome de exibição do **site**. Este será o nome do site do SharePoint.|
|id|String| A ID da sessão de **site**. Esta não é a ID do site real.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|site|[site](../resources/site.md)|O site do SharePoint associado ao **site**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
