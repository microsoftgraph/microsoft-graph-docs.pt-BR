---
title: Tipo de recurso attributeSet
description: Um objeto que representa um grupo de definições de atributos de segurança personalizados relacionados.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 958ecbd900a98cfe9f91bf5d7fe526b2f4050bfa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077140"
---
# <a name="attributeset-resource-type"></a>Tipo de recurso attributeSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto que representa um grupo de definições de atributos de segurança personalizados relacionados.

Até 500 `attributeSet` objetos podem ser definidos em um locatário. Não é possível renomeá-los ou excluídos.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar attributeSets](../api/directory-list-attributesets.md)|[Coleção attributeSet](../resources/attributeset.md)|Obter uma lista dos [objetos attributeSet](../resources/attributeset.md) e suas propriedades.|
|[Obter attributeSet](../api/attributeset-get.md)|[attributeSet](../resources/attributeset.md)|Leia as propriedades e as relações de um [objeto attributeSet.](../resources/attributeset.md)|
|[Criar attributeSet](../api/directory-post-attributesets.md)|[attributeSet](../resources/attributeset.md)|Crie um novo [objeto attributeSet.](../resources/attributeset.md)|
|[Atualizar attributeSet](../api/attributeset-update.md)|[attributeSet](../resources/attributeset.md)|Atualize as propriedades de um [objeto attributeSet.](../resources/attributeset.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição do conjunto de atributos. Pode ter até 128 caracteres e incluir caracteres Unicode. Pode ser alterado posteriormente.|
|id|Cadeia de caracteres|Identificador do conjunto de atributos que é exclusivo em um locatário. Pode ter até 32 caracteres e incluir caracteres Unicode. Não é possível conter espaços ou caracteres especiais. Não é possível alterá-los posteriormente. Maiúsculas de minúsculas.|
|maxAttributesPerSet|Int32|Número máximo de atributos de segurança personalizados que podem ser definidos neste conjunto de atributos. O valor padrão é `null`. Se não for especificado, o administrador poderá adicionar até o máximo de 500 atributos ativos por locatário. Pode ser alterado posteriormente.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attributeSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeSet",
  "description": "String",
  "id": "String (identifier)",
  "maxAttributesPerSet": "Integer"
}
```
