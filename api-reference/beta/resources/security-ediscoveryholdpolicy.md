---
title: Tipo de recurso ediscoveryHoldPolicy
description: '*tipo de recurso ediscoveryHoldPolicy'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8f40b4fe05858cfd37f401e640937867d617edcc
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945044"
---
# <a name="ediscoveryholdpolicy-resource-type"></a>Tipo de recurso ediscoveryHoldPolicy

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de retenção legal. As retenções legais são retenções vinculadas a um caso de Descoberta Eletrônica. As retenções legais não devem ser confundidas com retenções de retenção, que são usadas para controlar políticas de retenção para conteúdo do Microsoft 365. As retenções legais da Descoberta Eletrônica são para manter o conteúdo indefinidamente para litígio, investigações internas e outras ações legais em que o conteúdo precisa ser protegido contra exclusão. Para obter mais informações, [consulte Gerenciar retenções na Descoberta Eletrônica Avançada](/microsoft-365/compliance/managing-holds)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryHoldPolicies](../api/security-ediscoverycase-list-legalholds.md)|[coleção microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Obtenha uma lista dos [objetos ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) e suas propriedades.|
|[Criar ediscoveryHoldPolicy](../api/security-ediscoverycase-post-legalholds.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Crie um novo [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Obter ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-get.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Leia as propriedades e as relações de um [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Atualizar ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-update.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Atualize as propriedades de [um objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Excluir ediscoveryHoldPolicy](../api/security-ediscoverycase-delete-legalholds.md)|Nenhum|Exclui um [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Listar siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Obtenha os recursos siteSource da propriedade de navegação siteSources.|
|[Criar siteSource](../api/security-ediscoveryholdpolicy-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Crie um novo objeto siteSource.|
|[Listar userSources](../api/security-ediscoverycustodian-list-usersources.md)|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|Obtenha os recursos userSource da propriedade de navegação userSources.|
|[Criar userSource](../api/security-ediscoveryholdpolicy-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|Crie um novo objeto userSource.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|Cadeia de caracteres|Consulta KQL que especifica o conteúdo a ser mantido nos locais especificados. Para saber mais, consulte [consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta Eletrônica](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Para manter todo o conteúdo nos locais especificados, deixe **contentQuery em** branco. |
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a retenção legal. |
|createdDateTime|DateTimeOffset|A data e a hora em que a retenção legal foi criada. |
|descrição|Cadeia de caracteres| A descrição da retenção legal. |
|displayName|Cadeia de caracteres| O nome de exibição da retenção legal. |
|erros|Coleção String|Lista os erros ocorridos ao colocar a retenção. |
|id|Cadeia de caracteres|A ID do caso de Descoberta Eletrônica. Somente leitura. Herdado da [entidade](../resources/entity.md). |
|isEnabled|Booliano|Indica se a retenção está habilitada e mantendo ativamente o conteúdo. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|o usuário que modificou a retenção legal pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a retenção legal foi modificada pela última vez. |
|status|String|O status da retenção legal. Os valores possíveis são: `Pending`, `Error`, `Success`.|

### <a name="legalholdstatus-values"></a>Valores de legalHoldStatus

|Member|Descrição|
|:---|-----------|
|Pending| O processo de distribuição de retenção está em andamento. |
|Erro| Ocorreu um erro quando a retenção foi aplicada. |
|Êxito| A retenção foi aplicada com êxito e está mantendo o conteúdo especificado. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|**TODO: adicionar descrição**|
|userSources|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|**TODO: adicionar descrição**|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryHoldPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryHoldPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "isEnabled": "Boolean",
  "contentQuery": "String",
  "errors": [
    "String"
  ]
}
```

