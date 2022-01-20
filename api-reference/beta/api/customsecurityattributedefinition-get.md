---
title: Obter customSecurityAttributeDefinition
description: Leia as propriedades e as relações de um objeto customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 85d2fe3cdce1517a01fa2905fa7073540f56be24
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134032"
---
# <a name="get-customsecurityattributedefinition"></a>Obter customSecurityAttributeDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CustomSecAttributeAssignment.ReadWrite.All, CustomSecAttributeDefinition.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CustomSecAttributeAssignment.ReadWrite.All, CustomSecAttributeDefinition.ReadWrite.All|

O usuário inscreveu também deve ter uma das seguintes funções [de diretório:](/azure/active-directory/roles/permissions-reference)

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
GET /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-get-a-custom-security-attribute"></a>Exemplo: obter um atributo de segurança personalizado

O exemplo a seguir obtém uma única definição de atributo de segurança personalizada.

+ Conjunto de atributos: `Engineering`
+ Atributo: `ProjectDate`

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customsecurityattributedefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-customsecurityattributedefinition-powershell-snippets.md)]
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
HTTP/1.1 200 OK
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
