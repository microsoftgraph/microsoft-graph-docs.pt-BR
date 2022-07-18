---
title: Atualizar customSecurityAttributeDefinition
description: Atualize as propriedades de um objeto customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="update-customsecurityattributedefinition"></a>Atualizar customSecurityAttributeDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CustomSecAttributeDefinition.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CustomSecAttributeDefinition.ReadWrite.All|

O usuário inscreveu também deve ter a função de diretório Administrador de Definição [de Atributo](/azure/active-directory/roles/permissions-reference). Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|
|OData-Version|4.01. Opcional.|

> [!NOTE]
> Para atualizar os valores predefinidos para um atributo de segurança personalizado, você deve adicionar o header **OData-Version e atribuí-lo** o valor `4.01`.

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça *apenas* os valores das propriedades que devem ser atualizadas. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações em outros valores de propriedade.

A tabela a seguir especifica as propriedades que podem ser atualizadas. 

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição do atributo de segurança personalizado. Pode ter até 128 caracteres e incluir caracteres Unicode. Opcional.|
|status|String|Especifica se o atributo de segurança personalizado está ativo ou desativado. Os valores aceitáveis são `Available` e `Deprecated`. Opcional.|
|usePreDefinedValuesOnly|Booliano|Indica se somente valores predefinidos podem ser atribuídos ao atributo de segurança personalizado. Se definido como false, os valores de formulário livre serão permitidos. Pode ser alterado de true para false, mas não pode ser alterado de falso para verdadeiro. Se `type` estiver definido como Boolean, `usePreDefinedValuesOnly` não será possível definir como true. Opcional.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-a-custom-security-attribute"></a>Exemplo 1: atualizar um atributo de segurança personalizado

O exemplo a seguir atualiza a descrição de uma definição de atributo de segurança personalizada.

+ Conjunto de atributos: `Engineering`
+ Atributo: `ProjectDate`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate
Content-Type: application/json

{
  "description": "Target completion date (YYYY/MM/DD)",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-customsecurityattributedefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-the-predefined-values-for-a-custom-security-attribute"></a>Exemplo 2: atualizar os valores predefinidos para um atributo de segurança personalizado

O exemplo a seguir atualiza o status de um valor predefinido existente e adiciona um novo valor predefinido para uma definição de atributo de segurança personalizada.

+ Conjunto de atributos: `Engineering`
+ Atributo: `Project`
+ Tipo de dados de atributo: Coleção de cadeias de caracteres
+ Atualizar o valor predefinido: `Baker`
+ Novo valor predefinido: `Skagit`

> [!NOTE]
> Para essa solicitação, você deve adicionar o header **OData-Version e atribuí-lo** o valor `4.01`.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition_allowedvalues"
}
-->
``` msgraph-interactive
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project
Content-Type: application/json
OData-Version: 4.01

{
    "allowedValues@delta": [
        {
            "id": "Baker",
            "isActive": false
        },
        {
            "id": "Skagit",
            "isActive": true
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-deactivate-a-custom-security-attribute"></a>Exemplo 3: Desativar um atributo de segurança personalizado

O exemplo a seguir desativa uma definição de atributo de segurança personalizada.

+ Conjunto de atributos: `Engineering`
+ Atributo: `Project`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition_deactivate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project
Content-Type: application/json

{
  "status": "Deprecated"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-customsecurityattributedefinition-deactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-customsecurityattributedefinition-deactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-customsecurityattributedefinition-deactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-customsecurityattributedefinition-deactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-customsecurityattributedefinition-deactivate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-customsecurityattributedefinition-deactivate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
