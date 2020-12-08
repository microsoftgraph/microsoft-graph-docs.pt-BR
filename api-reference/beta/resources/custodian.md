---
title: tipo de recurso responsáveis
description: No contexto da descoberta eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597531"
---
# <a name="custodian-resource-type"></a>tipo de recurso responsáveis

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No contexto da descoberta eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar os responsáveis](../api/ediscoverycase-list-custodians.md)|coleção [responsáveis](../resources/custodian.md)|Obter uma lista de objetos **responsáveis** e suas propriedades.|
|[Criar responsáveis](../api/ediscoverycase-post-custodians.md)|[custódia](../resources/custodian.md)|Criar um novo objeto de **responsáveis** .|
|[Obter os responsáveis](../api/custodian-get.md)|[custódia](../resources/custodian.md)|Leia as propriedades e os relacionamentos de um objeto de **responsáveis** .|
|[Atualizar responsáveis](../api/custodian-update.md)|[custódia](../resources/custodian.md)|Atualizar as propriedades de um objeto de **responsáveis** .|
|[comunicado](../api/custodian-release.md)|Nenhum|Liberar um dos casos.|
|[ativar](../api/custodian-activate.md)|Nenhum|Reative os responsáveis que foram liberados de um caso e torne-os parte do caso novamente.|
|[Listar siteSources](../api/custodian-list-sitesources.md)|coleção de [sites de site](../resources/sitesource.md)|Obtenha os recursos de **site** da propriedade de navegação **siteSources** .|
|[Criar siteSources](../api/custodian-post-sitesources.md)|[site da site](../resources/sitesource.md)|Criar um novo objeto **sitery** .|
|[Listar unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)|Obtenha os recursos **unifiedGroupSource** da propriedade de navegação **unifiedGroupSources** .|
|[Criar unifiedGroupSources](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|Criar um novo objeto **unifiedGroupSource** .|
|[Listar usersources](../api/custodian-list-usersources.md)|coleção [username](../resources/usersource.md)|Obter os recursos de **username** da propriedade de navegação **usersources** .|
|[Criar usersources](../api/custodian-post-usersources.md)|[username](../resources/usersource.md)|Criar um novo objeto **username** .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Data e hora em que os responsáveis confirmaram uma notificação de bloqueio.|
|applyHoldToSources|Boolean|Identifica se as fontes dos responsáveis foram colocadas em espera durante a criação.|
|createdDateTime|DateTimeOffset|Data e hora em que os responsáveis foram adicionados ao caso.|
|displayName|String|Nome de exibição do responsáveis.|
|email|Cadeia de caracteres|Endereço de email do responsáveis.|
|id|String|A ID dos responsáveis no caso especificado. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do objeto responsáveis|
|releasedDateTime|DateTimeOffset|Data e hora em que os responsáveis foram liberados do caso.|
|status|custodianStatus|Status dos responsáveis. Os valores possíveis são: `active` e `released`.|

### <a name="custodianstatus-values"></a>valores de custodianStatus

|Member|Descrição|
|:----|-----------|
|active|O responsáveis é uma parte ativa do caso. |
|solta|Os responsáveis são liberados do caso.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|coleção de [sites de site](../resources/sitesource.md)|Entidade de fonte de dados para sites do SharePoint associados aos responsáveis.|
|unifiedGroupSources|coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)|Entidade de fonte de dados para grupos associados aos responsáveis.|
|usersources|coleção [username](../resources/usersource.md)|Entidade de fonte de dados para um dos responsáveis. Este é o contêiner para a caixa de correio de um dos responsáveis e o site do OneDrive for Business.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```
