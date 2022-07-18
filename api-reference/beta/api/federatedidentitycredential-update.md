---
title: Atualizar federatedIdentityCredential
description: Atualize as propriedades de um objeto federatedIdentityCredential.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 11ee8eb14f13398dcf322b1f2553f076e3db9038
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602753"
---
# <a name="update-federatedidentitycredential"></a>Atualizar federatedIdentityCredential
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) |  Application.ReadWrite.All |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /applications/{applicationId}/federatedIdentityCredentials/{federatedIdentityCredentialId}

PATCH /applications/{applicationId}/federatedIdentityCredentials/{federatedIdentityCredentialName}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça *apenas* os valores das propriedades que devem ser atualizadas. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações em outros valores de propriedade.

A tabela a seguir especifica as propriedades que podem ser atualizadas.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Público|Conjunto de cadeias de caracteres|A lista de audiências que podem aparecer no token emitido. O valor recomendado é `api://AzureADTokenExchange`. |
|descrição|Cadeia de caracteres|Uma descrição fornecida pelo usuário do que o federatedIdentityCredential é usado. |
|Emissor|Cadeia de caracteres|A URL do emissor confiável de entrada (Serviço de Token Seguro). Corresponde à declaração do emissor de um token de acesso. Por exemplo, com o cenário chaves gerenciadas pelo cliente, Azure AD é o emissor e um valor válido seria `https://login.microsoftonline.com/{tenantid}/v2.0`. A combinação dos valores do **emissor e** **da entidade** deve ser exclusiva no aplicativo. |
|assunto|String|<li>Para Azure AD emissor, o `objectId` do servicePrincipal (pode representar uma identidade gerenciada) que pode representar o aplicativo. O objeto associado a esse GUID precisa existir no locatário.</li><li>Para todos os outros emissores, uma cadeia de caracteres sem validação adicional</ul><br><br>A combinação dos valores do **emissor e** **da entidade** deve ser exclusiva no aplicativo.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_federatedidentitycredential"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/15be77d1-1940-43fe-8aae-94a78e078da0
Content-Type: application/json

{
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": "Updated description",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-federatedidentitycredential-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-federatedidentitycredential-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-federatedidentitycredential-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-federatedidentitycredential-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-federatedidentitycredential-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-federatedidentitycredential-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content

```

