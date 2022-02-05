---
title: Criar customSecurityAttributeDefinition
description: Crie um novo objeto customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="create-customsecurityattributedefinition"></a>Criar customSecurityAttributeDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CustomSecAttributeDefinition.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CustomSecAttributeDefinition.ReadWrite.All|

O usuário in-loco também deve ser atribuído ao Administrador de Definição de Atributo [função de diretório](/azure/active-directory/roles/permissions-reference. Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/customSecurityAttributeDefinitions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) .

A tabela a seguir mostra as propriedades que você pode configurar ao criar [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attributeSet|String|Nome do conjunto de atributos. Maiúsculas de minúsculas. Obrigatório.|
|description|String|Descrição do atributo de segurança personalizado. Pode ter até 128 caracteres e incluir caracteres Unicode. Não é possível conter espaços ou caracteres especiais. Pode ser alterado posteriormente. Opcional.|
|isCollection|Booliano|Indica se vários valores podem ser atribuídos ao atributo de segurança personalizado. Não é possível alterá-los posteriormente. Se `type` estiver definido como Boolean, `isCollection` não será possível definir como true. Obrigatório.|
|isSearchable|Booliano|Indica se os valores de atributo de segurança personalizados serão indexados para pesquisa em objetos atribuídos a valores de atributo. Não é possível alterá-los posteriormente. Obrigatório.|
|nome|String|Nome do atributo de segurança personalizado. Deve ser exclusivo em um conjunto de atributos. Pode ter até 32 caracteres e incluir caracteres Unicode. Não é possível conter espaços ou caracteres especiais. Não é possível alterá-los posteriormente. Maiúsculas de minúsculas. Obrigatório.|
|status|Cadeia de caracteres|Especifica se o atributo de segurança personalizado está ativo ou desativado. Os valores aceitáveis são `Available` e `Deprecated`. Pode ser alterado posteriormente. Obrigatório.|
|type|Cadeia de caracteres|Tipo de dados para os valores de atributo de segurança personalizados. Os tipos com suporte são `Boolean`, `Integer`e `String`. Não é possível alterá-los posteriormente. Obrigatório.|
|usePreDefinedValuesOnly|Booliano|Indica se somente valores predefinidos podem ser atribuídos ao atributo de segurança personalizado. Se definido como false, os valores de formulário livre serão permitidos. Posteriormente, pode ser alterado de true para false, mas não pode ser alterado de falso para verdadeiro. Se `type` estiver definido como Boolean, `usePreDefinedValuesOnly` não será possível definir como true. Obrigatório.|

A `id` propriedade é gerada automaticamente e não pode ser definida.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-a-custom-security-attribute"></a>Exemplo 1: Adicionar um atributo de segurança personalizado

O exemplo a seguir adiciona uma nova definição de atributo de segurança personalizada que é um único valor de formulário livre do tipo String.

+ Conjunto de atributos: `Engineering`
+ Atributo: `ProjectDate`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json

{
    "attributeSet":"Engineering",
    "description":"Target completion date",
    "isCollection":false,
    "isSearchable":true,
    "name":"ProjectDate",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-customsecurityattributedefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Target completion date",
    "id": "Engineering_ProjectDate",
    "isCollection": false,
    "isSearchable": true,
    "name": "ProjectDate",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": false
}
```

### <a name="example-2-add-a-custom-security-attribute-that-supports-multiple-predefined-values"></a>Exemplo 2: Adicionar um atributo de segurança personalizado que oferece suporte a vários valores predefinidos

O exemplo a seguir adiciona uma nova definição de atributo de segurança personalizada que oferece suporte a vários valores do tipo String predefinidos.

+ Conjunto de atributos: `Engineering`
+ Atributo: `Project`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition_v2"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json
Content-length: 310

{
    "attributeSet":"Engineering",
    "description":"Active projects for user",
    "isCollection":true,
    "isSearchable":true,
    "name":"Project",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-customsecurityattributedefinition-v2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-customsecurityattributedefinition-v2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-customsecurityattributedefinition-v2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-customsecurityattributedefinition-v2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-customsecurityattributedefinition-v2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-customsecurityattributedefinition-v2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Active projects for user",
    "id": "Engineering_Project",
    "isCollection": true,
    "isSearchable": true,
    "name": "Project",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": true
}
```

### <a name="example-3-add-a-custom-security-attribute-with-a-list-of-predefined-values"></a>Exemplo 3: Adicionar um atributo de segurança personalizado com uma lista de valores predefinidos

O exemplo a seguir adiciona uma nova definição de atributo de segurança personalizada com uma lista de valores predefinidos como uma coleção de cadeias de caracteres.

+ Conjunto de atributos: `Engineering`
+ Atributo: `Project`
+ Tipo de dados de atributo: Coleção de cadeias de caracteres
+ Valores predefinidos: `Alpine`, , `Baker``Cascade`

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition_allowedvalues"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json

{
    "attributeSet": "Engineering",
    "description": "Active projects for user",
    "isCollection": true,
    "isSearchable": true,
    "name": "Project",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": true,
    "allowedValues": [
        {
            "id": "Alpine",
            "isActive": true
        },
        {
            "id": "Baker",
            "isActive": true
        },
        {
            "id": "Cascade",
            "isActive": true
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Active projects for user",
    "id": "Engineering_Project",
    "isCollection": true,
    "isSearchable": true,
    "name": "Project",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": true
}
```
