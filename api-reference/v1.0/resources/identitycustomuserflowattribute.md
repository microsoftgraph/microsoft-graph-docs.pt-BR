---
title: Tipo de recurso identityCustomUserFlowAttribute
description: Representa um atributo de fluxo de usuário personalizado em locatários do Azure Active Directory que podem ser usados em um fluxo de usuário de autoatenduro.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2bb354ab8028a6d3ca96418c4b0566ea6fe195ef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882861"
---
# <a name="identitycustomuserflowattribute-resource-type"></a>Tipo de recurso identityCustomUserFlowAttribute

Namespace: microsoft.graph

Representa um atributo de fluxo de usuário personalizado em locatários do Azure Active Directory que podem ser usados em um fluxo de usuário de autoatenduro. Esses atributos não podem ser modificados e são somente leitura.

Herda de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do atributo de fluxo do usuário. Esse é um atributo somente leitura criado automaticamente. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|O nome de exibição do atributo de fluxo do usuário. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|description|String|A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|userFlowAttributeType|identityUserFlowAttributeType|O tipo do atributo de fluxo do usuário. Esse é um atributo somente leitura que é definido automaticamente. O valor dessa propriedade será `custom` . Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).|
|dataType|identityUserFlowAttributeDataType|O tipo de dados do atributo de fluxo do usuário. Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado. Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`. Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
