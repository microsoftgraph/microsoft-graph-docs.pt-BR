---
title: Listar allowedValues
description: Obter uma lista dos objetos allowedValue e suas propriedades.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="list-allowedvalues"></a>Listar allowedValues
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos allowedValue](../resources/allowedvalue.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CustomSecAttributeDefinition.Read.All, CustomSecAttributeDefinition.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CustomSecAttributeDefinition.Read.All, CustomSecAttributeDefinition.ReadWrite.All|

O usuário inscreveu também deve ter uma das seguintes funções [de diretório](/azure/active-directory/roles/permissions-reference):

+ Leitor de Atribuição de Atributo
+ Leitor de Definição de Atributo
+ Administrador de Atribuição de Atributo
+ Administrador de Definição de Atributo

Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues
```


## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos parâmetros `$select` de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção [de objetos allowedValue](../resources/allowedvalue.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-get-all-predefined-values"></a>Exemplo: Obter todos os valores predefinidos

O exemplo a seguir obtém todos os valores predefinidos para uma definição de atributo de segurança personalizada.

+ Conjunto de atributos: `Engineering`
+ Atributo: `Project`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_allowedvalue"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-allowedvalue-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-allowedvalue-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-allowedvalue-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-allowedvalue-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-allowedvalue-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-allowedvalue-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.allowedValue)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions('Engineering_Project')/allowedValues",
    "value": [
        {
            "id": "Cascade",
            "isActive": true
        },
        {
            "id": "Baker",
            "isActive": true
        },
        {
            "id": "Alpine",
            "isActive": true
        }
    ]
}
```
