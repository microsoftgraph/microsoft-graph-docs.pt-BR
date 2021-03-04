---
title: Tipo de recurso legalHold
description: Tipo de recurso legalHold
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa13783de13c216d8ec89aca67218e3eec56bfc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445927"
---
# <a name="legalhold-resource-type"></a>Tipo de recurso legalHold

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ressução legal. Os ressarces legais são ressarces que estão vinculados a um caso de Descoberta E. Os retenções legais não devem ser confundidos com retenções de retenção, que são usadas para controlar políticas de retenção para conteúdo do Microsoft 365. As resguardas legais de descoberta de eDiscovery são para manter o conteúdo indefinidamente para litígio, investigações internas e outras ações legais em que o conteúdo precisa ser protegido contra exclusão. Para obter mais informações, consulte [Manage holds in Advanced eDiscovery](/microsoft-365/compliance/managing-holds)

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar legalHolds](../api/ediscovery-case-list-legalholds.md)|[coleção microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Obter uma lista dos  **objetos legalHold** e suas propriedades.|
|[Criar legalHold](../api/ediscovery-case-post-legalholds.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Crie um novo **objeto legalHold.**|
|[Obter legalHold](../api/ediscovery-legalhold-get.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Leia as propriedades e as relações de um **objeto legalHold.**|
|[Atualizar legalHold](../api/ediscovery-legalhold-update.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Atualize as propriedades de um **objeto legalHold.**|
|[Excluir legalHold](../api/ediscovery-legalhold-delete.md)|Nenhum(a)|**Exclua um objeto legalHold.**|
|[Listar siteSources](../api/ediscovery-legalhold-list-sitesources.md)|[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Obter a lista [de objetos siteSource](../resources/ediscovery-sitesource.md) associados a uma resserção legal.|
|[Criar siteSource](../api/ediscovery-legalhold-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Crie um novo objeto siteSource.|
|[Listar userSources](../api/ediscovery-legalhold-list-usersources.md)|[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Obter a lista de [objetos userSource](../resources/ediscovery-usersource.md) associados a uma responsabilidade legal.|
|[Criar userSource](../api/ediscovery-legalhold-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Crie um novo **objeto userSource.**|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|String|Consulta KQL que especifica o conteúdo a ser mantido nos locais especificados. Para saber mais, confira [Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta De Conteúdo.](/microsoft-365/compliance/keyword-queries-and-search-conditions)  Para manter todo o conteúdo nos locais especificados, deixe **contentQuery em** branco. |
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a responsabilidade legal. |
|createdDateTime|DateTimeOffset|A data e a hora em que a ressução legal foi criada. |
|descrição|String| A descrição de espera legal. |
|displayName|String| O nome de exibição da ressução legal. |
|erros|Coleção de cadeias de caracteres|Lista todos os erros que aconteceram durante a colocação da espera. |
|id|String|A ID do caso de Descoberta e. Somente leitura. Herdado da [entidade](../resources/entity.md). |
|isEnabled|Booliano|Indica se a espera está habilitada e mantendo o conteúdo ativamente. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|o usuário que modificou pela última vez a responsabilidade legal.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a ressução legal foi modificada pela última vez. |
|status|microsoft.graph.ediscovery.legalHoldStatus|O status da ressução legal. Os valores possíveis são: `Pending`, `Error`, `Success`, `UnknownFutureValue`.|

### <a name="legalholdstatus-values"></a>valores legalHoldStatus

|Member|Descrição|
|:---|-----------|
|Pending| O processo de distribuição de espera está em andamento. |
|Erro| Houve um erro quando a espera foi aplicada. Para obter detalhes, consulte a propriedade errors do objeto legalHold. |
|Êxito| A espera foi aplicada com êxito e está segurando o conteúdo especificado. |

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|siteSources|[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Entidade de fonte de dados para sites do SharePoint associados à responsabilidade legal. |
|userSources|[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)| Entidade de fonte de dados para uma responsabilidade legal. Este é o contêiner para uma caixa de correio e um site do OneDrive for Business.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.legalHold",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "String (identifier)",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
