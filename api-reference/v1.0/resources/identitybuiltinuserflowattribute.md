---
title: Tipo de recurso identityBuiltInUserFlowAttribute
description: Representa um atributo de fluxo de usuário integrado Azure Active Directory locatários que podem ser usados em um fluxo de usuário de autoatendido.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ba728475ea83c7497022412ac59bf047d8f7b57a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098955"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a>Tipo de recurso identityBuiltInUserFlowAttribute

Namespace: microsoft.graph

Representa um atributo de fluxo de usuário integrado Azure Active Directory locatários que podem ser usados em um fluxo de usuário de autoatendido. Esses atributos não podem ser modificados e são somente leitura.

Herda de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do atributo de fluxo do usuário. Esse é um atributo somente leitura criado automaticamente. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|O nome de exibição do atributo de fluxo do usuário. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md). Somente leitura.|
|description|String|A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md). Somente leitura.|
|userFlowAttributeType|identityUserFlowAttributeType|O tipo do atributo de fluxo do usuário. Esse é um atributo somente leitura que é definido automaticamente. O valor dessa propriedade será `builtIn` . Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md). Somente leitura.|
|dataType|identityUserFlowAttributeDataType|O tipo de dados do atributo de fluxo do usuário. Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado. Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md). Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
