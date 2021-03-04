---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 3e8707627b09784972a1a578fe4b6b84a623f4dd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440238"
---
# <a name="identityuserflowattribute-resource-type"></a>tipo de recurso identityUserFlowAttribute

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD) e em um locatário do Azure AD B2C.

Configurar os atributos de fluxo de usuário no seu Azure AD ou no Azure AD B2C permite que você colete informações sobre um usuário durante a inscrição. Você pode optar por coletar um conjunto de atributos interno. Por exemplo, o nome, o sobrenome, a cidade e o CEP. Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório. Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityuserflowattribute-list.md)|coleção identityUserFlowAttributes |Recuperar todos os atributos internos de fluxo de usuário.|
|[Create](../api/identityuserflowattribute-post.md)|identityUserFlowAttribute|Criar um novo atributo de fluxo de usuário personalizado.|
|[Get](../api/identityuserflowattribute-get.md) |identityUserFlowAttribute|Recuperar as propriedades de um atributo de fluxo de usuário.|
|[Atualizar](../api/identityuserflowattribute-update.md)|Nenhum(a)|Atualizar um atributo de fluxo de usuário personalizado.|
|[Delete](../api/identityuserflowattribute-delete.md)|Nenhum(a)|Excluir um atributo de fluxo de usuário personalizado.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|String|O identificador do atributo de fluxo do usuário. Esse é um atributo somente leitura criado automaticamente.|
|displayName|String|O nome de exibição do atributo de fluxo do usuário.|
|descrição|String|A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.|
|userFlowAttributeType|String|O tipo do atributo de fluxo do usuário. Esse é um atributo somente leitura que é definido automaticamente. Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.|
|dataType|Cadeia de caracteres|O tipo de dados do atributo de fluxo do usuário. Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado. Os valores com suporte para **tipo de dados** são:<br/><ul><li>`string` -indica que o tipo de dados para identityUserFlowAttribute é uma cadeia de caracteres. </li><li>`boolean` -indica que o tipo de dados para identityUserFlowAttribute é um booleano.</li><li>`int64` -indica que o tipo de dados para identityUserFlowAttribute é um número inteiro.</li></ul>|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
