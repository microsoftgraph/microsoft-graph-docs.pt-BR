---
title: Listar accessPackageResourceEnvironments
description: Recupere uma lista de objetos accessPackageResourceEnvironment.
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1b8a56a9f5e9c01836b61a4974a44c66f8429ac8
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805050"
---
# <a name="list-accesspackageresourceenvironments"></a>Listar accessPackageResourceEnvironments
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="query-parameters"></a>Parâmetros de consulta

Este método requer o parâmetro `$filter` [de consulta OData](/graph/query-parameters). Você deve aplicar para `$filter` recuperar a **origemSystem** atribuída ao valor `SharePointOnline`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accesspackageresourceenvironment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-accesspackageresourceenvironment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

