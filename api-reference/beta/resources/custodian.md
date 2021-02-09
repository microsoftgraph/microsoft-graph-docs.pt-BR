---
title: tipo de recurso custodian
description: No contexto da Descoberta eDiscovery, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157677"
---
# <a name="custodian-resource-type"></a>tipo de recurso custodian

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No contexto da Descoberta eDiscovery, representa um usuário e todos os seus ativos digitais, como emails e documentos.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar custodiantes](../api/ediscoverycase-list-custodians.md)|[coleção custodian](../resources/custodian.md)|Obter uma lista de **objetos custodiantes** e suas propriedades.|
|[Criar custodiatário](../api/ediscoverycase-post-custodians.md)|[custodian](../resources/custodian.md)|Criar um novo **objeto custodiante.**|
|[Obter custodian](../api/custodian-get.md)|[custodian](../resources/custodian.md)|Leia as propriedades e os relacionamentos de um **objeto custodiante.**|
|[Atualizar custodian](../api/custodian-update.md)|[custodian](../resources/custodian.md)|Atualizar as propriedades de **um objeto custodiante.**|
|[release](../api/custodian-release.md)|Nenhum(a)|Libere um custodiante de uma ocorrência.|
|[ativar](../api/custodian-activate.md)|Nenhum(a)|Reativar um custodiante que foi liberado de uma ocorrência e torná-lo parte do caso novamente.|
|[Listar siteSources](../api/custodian-list-sitesources.md)|[coleção siteSource](../resources/sitesource.md)|Obter os **recursos siteSource** da **propriedade de navegação siteSources.**|
|[Criar siteSources](../api/custodian-post-sitesources.md)|[siteSource](../resources/sitesource.md)|Criar um novo **objeto siteSource.**|
|[Listar unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|[Coleção unifiedGroupSource](../resources/unifiedgroupsource.md)|Obter os **recursos unifiedGroupSource** da **propriedade de navegação unifiedGroupSources.**|
|[Criar unifiedGroupSources](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|Crie um novo **objeto unifiedGroupSource.**|
|[Listar userSources](../api/custodian-list-usersources.md)|[Coleção userSource](../resources/usersource.md)|Obter os **recursos userSource** da **propriedade de navegação userSources.**|
|[Criar userSources](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|Crie um novo **objeto userSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Data e hora em que o custodiado reconheceu uma notificação de espera.|
|applyHoldToSources|Boolean|Identifica se as fontes de um custodiador foram colocadas em espera durante a criação.|
|createdDateTime|DateTimeOffset|Data e hora em que o custodiante foi adicionado à ocorrência.|
|displayName|String|Nome de exibição do custodiado.|
|email|Cadeia de caracteres|Endereço de email do custodiatário.|
|id|String|A ID do custodiante no caso especificado. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o objeto custodiante foi modificado pela última vez|
|releasedDateTime|DateTimeOffset|Data e hora em que o custodiante foi liberado da ocorrência.|
|status|custodianStatus|Status do custodiatário. Os valores possíveis são: `active` e `released`.|

### <a name="custodianstatus-values"></a>valores de custodianStatus

|Member|Descrição|
|:----|-----------|
|ativo|Custodian é uma parte ativa da ocorrência. |
|released|Custodian is released from the case.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|[coleção siteSource](../resources/sitesource.md)|Entidade de fonte de dados para sites do SharePoint associados ao custodiante.|
|unifiedGroupSources|[Coleção unifiedGroupSource](../resources/unifiedgroupsource.md)|Entidade de fonte de dados para grupos associados ao custodiante.|
|userSources|[Coleção userSource](../resources/usersource.md)|Entidade de fonte de dados para um custodiante. Esse é o contêiner da caixa de correio de um responsável e do site do OneDrive for Business.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
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
