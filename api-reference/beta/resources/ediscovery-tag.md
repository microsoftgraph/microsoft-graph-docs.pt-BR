---
title: tipo de recurso tag
description: Representa uma marca eDiscovery, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e não responsivo
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445944"
---
# <a name="tag-resource-type"></a>tipo de recurso tag

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma marca eDiscovery, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e não responsivo.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar marcas](../api/ediscovery-case-list-tags.md)|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Obter uma lista dos objetos **de marca** e suas propriedades.|
|[Criar marca](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Crie um novo **objeto tag.**|
|[Obter marca](../api/ediscovery-tag-get.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Leia as propriedades e as relações de um **objeto tag.**|
|[Marca de atualização](../api/ediscovery-tag-update.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Atualize as propriedades de um **objeto tag.**|
|[Excluir marca](../api/ediscovery-tag-delete.md)|Nenhum(a)|Exclua **um objeto tag.**|
|[asHierarchy](../api/ediscovery-tag-ashierarchy.md)|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Lista todas as marcas, incluindo a hierarquia.|
|[Listar childTags](../api/ediscovery-tag-childtags.md)|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Obter uma lista de objetos **de marca** filho associados a uma marca.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|childSelectability|[microsoft.graph.ediscovery.childSelectability](../resources/ediscovery-tag.md#childselectability-values)|Indica se uma única ou várias marcas filho podem ser associadas a um documento. Os valores possíveis são: `One` e `Many`.  Esse valor controla se o UX apresenta as marcas como caixas de seleção ou um grupo de botões de rádio.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a marca.|
|descrição|String|A descrição da marca.|
|displayName|String|Nome de exibição da marca.|
|id|String|Identificador exclusivo da marca.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a marca foi modificada pela última vez.|

### <a name="childselectability-values"></a>valores childSelectability

|Member|Descrição|
|:----|-----------|
|Um|Somente um filho pode ser selecionado. Isso corresponde a uma interface do usuário que apresenta as marcas com botões de rádio.|
|Muitos|Zero ou muitos filhos podem ser selecionados. Isso corresponde a uma interface do usuário que apresenta as marcas com caixas de seleção.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|childTags|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Retorna as marcas que são filho de uma marca.|
|primário|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Retorna a marca pai da marca especificada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
