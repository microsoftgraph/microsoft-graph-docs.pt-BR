---
title: tipo de recurso custodiado
description: No contexto da Descoberta Digital, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0d71542b796f5256f21e19a886533e3a88e1d7ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446173"
---
# <a name="custodian-resource-type"></a>tipo de recurso custodiado

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No contexto da Descoberta Digital, representa um usuário e todos os seus ativos digitais, como emails e documentos.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar custodiantes](../api/ediscovery-case-list-custodians.md)|[coleção microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Obter uma lista de **objetos custodiantes** e suas propriedades.|
|[Criar custodiatário](../api/ediscovery-case-post-custodians.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Crie um novo **objeto custodiante.**|
|[Obter custodiatário](../api/ediscovery-custodian-get.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Leia as propriedades e as relações de um **objeto custodiante.**|
|[Atualizar custodiatário](../api/ediscovery-custodian-update.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Atualize as propriedades de **um objeto custodiante.**|
|[release](../api/ediscovery-custodian-release.md)|Nenhum(a)|Libere um custodiante de um caso.|
|[activate](../api/ediscovery-custodian-activate.md)|Nenhum(a)|Reativar um custodiante que foi liberado de um caso e torná-lo parte do caso novamente.|
|[Listar siteSources](../api/ediscovery-custodian-list-sitesources.md)|[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Obter os **recursos siteSource** associados ao custodiado.|
|[Criar siteSources](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Crie um novo **objeto siteSource.**|
|[Listar unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[coleção microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Obter a lista de **recursos unifiedGroupSource** associados ao custodiado.|
|[Criar unifiedGroupSources](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Crie um novo **objeto unifiedGroupSource.**|
|[Listar userSources](../api/ediscovery-custodian-list-usersources.md)|[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Obter a lista **de recursos userSource** associados ao custodiado.|
|[Criar userSources](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Crie um novo **objeto userSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Data e hora em que o custodiado reconheceu uma notificação de responsabilidade.|
|applyHoldToSources|Booliano|Identifica se as fontes de um custodiador foram colocadas em espera durante a criação.|
|createdDateTime|DateTimeOffset|Data e hora em que o custodiante foi adicionado ao caso.|
|displayName|String|Nome de exibição do custodiado.|
|email|Cadeia de caracteres|Endereço de email do custodiado.|
|id|String|A ID do custodiante no caso especificado. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o objeto custodiante foi modificado pela última vez|
|releasedDateTime|DateTimeOffset|Data e hora em que o custodiante foi liberado do caso.|
|status|microsoft.graph.ediscovery.custodianStatus|Status do custodiado. Os valores possíveis são: `active` e `released`.|

### <a name="custodianstatus-values"></a>valores custodianStatus

|Member|Descrição|
|:----|-----------|
|active|O custodiante é uma parte ativa do caso. |
|released|O custodiante é liberado do caso.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Entidade de fonte de dados para sites do SharePoint associados ao custodiante.|
|unifiedGroupSources|[coleção microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Entidade de fonte de dados para grupos associados ao custodiante.|
|userSources|[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Entidade de fonte de dados para um custodiante. Este é o contêiner para a caixa de correio de um custodiado e o site do OneDrive for Business.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.custodian",
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
