---
title: Tipo de recurso ediscoveryReviewTag
description: Representa uma marca de Descoberta Eletrônica, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e sem resposta
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4bd787ed238fdd7c365b913a98d1129d2b80b35d
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838595"
---
# <a name="ediscoveryreviewtag-resource-type"></a>Tipo de recurso ediscoveryReviewTag

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma marca de Descoberta Eletrônica, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e sem resposta.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryReviewTags](../api/security-ediscoverycase-list-tags.md)|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Obtenha uma lista dos [objetos ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) e suas propriedades.|
|[Criar ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Crie um novo [objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Obter ediscoveryReviewTag](../api/security-ediscoveryreviewtag-get.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Leia as propriedades e as relações de um [objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Atualizar ediscoveryReviewTag](../api/security-ediscoveryreviewtag-update.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Atualize as propriedades de [um objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Excluir ediscoveryReviewTag](../api/security-ediscoverycase-delete-tags.md)|Nenhum|[Exclua um objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md).|
|[asHierarchy](../api/security-ediscoveryreviewtag-ashierarchy.md)|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Listar marcas organizadas como hierarquia.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|childSelectability|microsoft.graph.security.childSelectability|Indica se uma única ou várias marcas filho podem ser associadas a um documento. Os valores possíveis são: `One` e `Many`.  Esse valor controla se a experiência do usuário apresenta as marcas como caixas de seleção ou um grupo de botões de opção.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a marca.|
|descrição|String|A descrição da marca.|
|displayName|String|Nome de exibição da marca.|
|id|String|Identificador exclusivo da marca.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a marca foi modificada pela última vez.|

### <a name="childselectability-values"></a>valores childSelectability

|Member|Descrição|
|:----|-----------|
|Um|Somente um filho pode ser selecionado. Isso corresponde a uma interface do usuário que apresenta as marcas com botões de opção.|
|Muitos|Zero ou muitos filhos podem ser selecionados. Isso corresponde a uma interface do usuário que apresenta as marcas com caixas de seleção.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|childTags|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Retorna as marcas que são um filho de uma marca.|
|primário|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Retorna a marca pai da marca especificada.|
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "childSelectability": "String"
}
```

