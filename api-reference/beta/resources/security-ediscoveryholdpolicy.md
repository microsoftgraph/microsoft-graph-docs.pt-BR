---
title: Tipo de recurso ediscoveryHoldPolicy
description: '*tipo de recurso ediscoveryHoldPolicy'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 46207724e8f8b2b23dc3d42543de8af67390ce87
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837559"
---
# <a name="ediscoveryholdpolicy-resource-type"></a>Tipo de recurso ediscoveryHoldPolicy

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de retenção legal. As retenções legais são retenções vinculadas a um caso de Descoberta Eletrônica. As retenções legais não devem ser confundidas com retenções de retenção, que são usadas para controlar políticas de retenção para conteúdo do Microsoft 365. As retenções legais da Descoberta Eletrônica são para manter o conteúdo indefinidamente para litígio, investigações internas e outras ações legais em que o conteúdo precisa ser protegido contra exclusão. Para obter mais informações, [consulte Gerenciar retenções na Descoberta Eletrônica (Premium)](/microsoft-365/compliance/managing-holds)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryHoldPolicies](../api/security-ediscoverycase-list-legalholds.md)|[coleção microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Obtenha uma lista dos [objetos ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) e suas propriedades.|
|[Criar ediscoveryHoldPolicy](../api/security-ediscoverycase-post-legalholds.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Crie um novo [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Obter ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-get.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Leia as propriedades e as relações de um [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Atualizar ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-update.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Atualize as propriedades de [um objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Excluir ediscoveryHoldPolicy](../api/security-ediscoverycase-delete-legalholds.md)|Nenhum|[Exclua um objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md).|
|[Listar siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Obtenha os recursos siteSource da propriedade de navegação siteSources.|
|[Criar siteSource](../api/security-ediscoveryholdpolicy-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Crie um novo objeto siteSource.|
|[Listar userSources](../api/security-ediscoverycustodian-list-usersources.md)|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|Obtenha os recursos userSource da propriedade de navegação userSources.|
|[Criar userSource](../api/security-ediscoveryholdpolicy-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|Crie um novo objeto userSource.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|String|Consulta KQL que especifica o conteúdo a ser mantido nos locais especificados. Para saber mais, consulte [consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta Eletrônica](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Para manter todo o conteúdo nos locais especificados, deixe **contentQuery em** branco. |
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a retenção legal. |
|createdDateTime|DateTimeOffset|A data e a hora em que a retenção legal foi criada. |
|descrição|String| A descrição da retenção legal. |
|displayName|String| O nome de exibição da retenção legal. |
|erros|String collection|Lista os erros ocorridos ao colocar a retenção. |
|id|String|A ID do caso de Descoberta Eletrônica. Somente leitura. Herdado da [entidade](../resources/entity.md). |
|isEnabled|Booliano|Indica se a retenção está habilitada e mantendo ativamente o conteúdo. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|o usuário que modificou a retenção legal pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a retenção legal foi modificada pela última vez. |
|status|microsoft.graph.security.policyStatus|O status da retenção legal. Os valores possíveis são: `Pending`, `Error`, `Success`.|

### <a name="policystatus-values"></a>Valores policyStatus

|Member|Descrição|
|:---|-----------|
|Pending| O processo de distribuição de retenção está em andamento. |
|Erro| Ocorreu um erro quando a retenção foi aplicada. |
|Êxito| A retenção foi aplicada com êxito e está mantendo o conteúdo especificado. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|[Coleção microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Fontes de dados que representam sites do SharePoint.|
|userSources|[Coleção microsoft.graph.security.userSource](../resources/security-usersource.md)|Fontes de dados que representam caixas de correio do Exchange.|

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

