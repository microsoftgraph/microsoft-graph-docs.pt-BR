---
title: Criar attributeSet
description: Crie um novo objeto attributeSet.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 33a8c33e68df4df9cb141b9d098a2663f452cbbb
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226481"
---
# <a name="create-attributeset"></a>Criar attributeSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto attributeSet.](../resources/attributeset.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|CustomSecAttributeDefinition.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CustomSecAttributeDefinition.ReadWrite.All|

O usuário inscreveu também deve ter a função de diretório Administrador de Definição [de Atributo.](/azure/active-directory/roles/permissions-reference) Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/attributeSets
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto attributeSet.](../resources/attributeset.md)

A tabela a seguir mostra as propriedades que você pode configurar ao criar [o atributoSet](../resources/attributeset.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição do conjunto de atributos. Pode ter até 128 caracteres e incluir caracteres Unicode. Pode ser alterado posteriormente. Opcional.|
|id|String|Identificador do conjunto de atributos que é exclusivo em um locatário. Pode ter até 32 caracteres e incluir caracteres Unicode. Não é possível conter espaços ou caracteres especiais. Não é possível alterá-los posteriormente. Maiúsculas de minúsculas. Obrigatório.|
|maxAttributesPerSet|Int32|Número máximo de atributos de segurança personalizados que podem ser definidos neste conjunto de atributos. O valor padrão é `null`. Se não for especificado, o administrador poderá adicionar até o máximo de 500 atributos ativos por locatário. Pode ser alterado posteriormente. Opcional.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [attributeSet](../resources/attributeset.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-add-an-attribute-set"></a>Exemplo: Adicionar um conjunto de atributos

O exemplo a seguir adiciona um novo conjunto de atributos chamado `Engineering` .

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_attributeset"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/attributeSets
Content-Type: application/json

{
    "id":"Engineering",
    "description":"Attributes for engineering team",
    "maxAttributesPerSet":25
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-attributeset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-attributeset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-attributeset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-attributeset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-attributeset-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets/$entity",
    "description": "Attributes for engineering team",
    "id": "Engineering",
    "maxAttributesPerSet": 25
}
```
