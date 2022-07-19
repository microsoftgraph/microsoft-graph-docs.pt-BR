---
title: Tipo de recurso ediscoveryCustodian
description: No contexto da Descoberta Eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 734430121fed536e77250ba17eaedc95029ca4bf
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839112"
---
# <a name="ediscoverycustodian-resource-type"></a>Tipo de recurso ediscoveryCustodian

Namespace: microsoft.graph.security



No contexto da Descoberta Eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryCustodians](../api/security-ediscoverycase-list-custodians.md)|[coleção microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Obtenha uma lista dos [objetos ediscoveryCustodian](../resources/security-ediscoverycustodian.md) e suas propriedades.|
|[Criar ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Crie um novo [objeto ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .|
|[Obter ediscoveryCustodian](../api/security-ediscoverycustodian-get.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Leia as propriedades e as relações de [um objeto ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .|
|[updateIndex](../api/security-ediscoverycustodian-updateindex.md)|Dispara uma indexOperation para tornar um guardião e fontes associadas pesquisáveis.|
|[Ativar](../api/security-ediscoverycustodian-activate.md)|Nenhum|Reative um guardião de um caso.|
|[Lançamento](../api/security-ediscoverycustodian-release.md)|Nenhum|Libere um guardião de um caso.|
|[applyHold](../api/security-ediscoverycustodian-applyhold.md)|Nenhum|Inicie o processo de aplicação de retenção aos custodiantes da Descoberta Eletrônica.|
|[removeHold](../api/security-ediscoverycustodian-removehold.md)|Nenhum|Inicie o processo de remoção da retenção dos custodiantes da Descoberta Eletrônica.|
|[Listar ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[coleção microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Obtenha uma lista da [descoberta eletrônicaIndexOperation associada](../resources/security-ediscoveryindexoperation.md) a [um ediscoveryCustodian](../resources/security-ediscoverycustodian.md).|
|[Listar siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Obtenha os recursos siteSource da propriedade de navegação siteSources.|
|[Criar siteSource](../api/security-ediscoverycustodian-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Crie um novo [objeto siteSource](../resources/security-sitesource.md) associado a [um guardião de Descoberta Eletrônica](../resources/security-ediscoverycustodian.md).|
|[Listar unifiedGroupSources](../api/security-ediscoverycustodian-list-unifiedgroupsources.md)|[Coleção microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Obtenha os recursos unifiedGroupSource da propriedade de navegação unifiedGroupSources.|
|[Criar unifiedGroupSource](../api/security-ediscoverycustodian-post-unifiedgroupsources.md)|[microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Crie um novo [objeto unifiedGroupSource](../resources/security-unifiedgroupsource.md) associado a [um guardião de Descoberta Eletrônica](../resources/security-ediscoverycustodian.md).|
|[Listar userSources](../api/security-ediscoverycustodian-list-usersources.md)|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|Obtenha os recursos userSource da propriedade de navegação userSources.|
|[Criar userSource](../api/security-ediscoverycustodian-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|Crie um novo [objeto userSource](../resources/security-usersource.md) associado a [um guardião de Descoberta Eletrônica](../resources/security-ediscoverycustodian.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Data e hora em que o guardião reconheceu uma notificação de suspensão.|
|createdDateTime|DateTimeOffset|Data e hora em que o guardião foi adicionado ao caso.|
|displayName|String|Nome de exibição do guardião.|
|email|Cadeia de caracteres|Email endereço do guardião.|
|id|String|A ID do guardião no caso especificado. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o objeto custodiante foi modificado pela última vez|
|releasedDateTime|DateTimeOffset|Data e hora em que o guardião foi liberado do caso.|
|status|microsoft.graph.security.custodianStatus|Status do guardião. Os valores possíveis são: `active` e `released`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de suspensão do guardião. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

### <a name="custodianstatus-values"></a>valores custodianStatus

|Nome|Descrição|
|:----|-----------|
|Ativo|Custodiante é uma parte ativa do caso. |
|Lançado|Custodiante está liberado do caso.|

### <a name="custodianholdstatus-values"></a>valores de custodianHoldStatus

|Nome|Descrição|
|:----|-----------|
|notApplied|O guardião não está em espera (todas as fontes nele não estão em espera).|
|Aplicado|O guardião está em espera (todas as fontes estão em espera).|
|Aplicação|O guardião está aplicando o estado de retenção (operação applyHold disparada).|
|Remover|O guardião está removendo o estado de retenção (operação removeHold disparada).|
|Parcial|O guardião está em estado misto em que algumas fontes estão em espera e outras não estão em retenção ou estado de erro.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Entidade de operação que representa a indexação mais recente para o guardião.|
|siteSources|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Entidade de fonte de dados para sites do SharePoint associados ao guardião.|
|unifiedGroupSources|[Coleção microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Entidade de fonte de dados para grupos associados ao guardião.|
|userSources|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|Entidade de fonte de dados para um guardião. Este é o contêiner para a caixa de correio de um guardião e OneDrive for Business site.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCustodian",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCustodian",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "email": "String",
  "acknowledgedDateTime": "String (timestamp)"
}
```

