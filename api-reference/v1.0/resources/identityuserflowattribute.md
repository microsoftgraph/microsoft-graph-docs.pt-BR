---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: af3ec2a762fc0252da929d863917ba6cd274ba95
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882783"
---
# <a name="identityuserflowattribute-resource-type"></a>tipo de recurso identityUserFlowAttribute

Namespace: microsoft.graph

Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD).

Configurar os atributos de fluxo de usuário no seu locatário do Azure AD permite que você colete informações sobre um usuário durante a inscrição. Você pode escolher coletar um conjunto interno de atributos. Por exemplo, nome, sobrenome, cidade e CEP. Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório. Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).

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
|userFlowAttributeType|identityUserFlowAttributeType|O tipo do atributo de fluxo do usuário. Esse é um atributo somente leitura que é definido automaticamente. Dependendo do tipo de atributo, os valores desta propriedade serão `builtIn`, `custom` ou `required`.|
|dataType|identityUserFlowAttributeDataType|O tipo de dados do atributo de fluxo do usuário. Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado. Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.|

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
