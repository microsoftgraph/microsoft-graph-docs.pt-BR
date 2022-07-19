---
title: Criar ediscoveryHoldPolicy
description: Crie um novo objeto ediscoveryHoldPolicy.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8cdbd719808d314d40d2c3f406b467bd163a19db
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838764"
---
# <a name="create-ediscoveryholdpolicy"></a>Criar ediscoveryHoldPolicy
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/legalHolds
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON [do objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .

Você pode especificar as propriedades a seguir ao criar **um ediscoveryHoldPolicy**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da política de retenção legal. Obrigatório.|
|description|String|A descrição da política de retenção legal. Opcional.|
|contentQuery|String|A consulta de conteúdo da política de retenção legal. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryholdpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalHolds
Content-Type: application/json

{
    "displayname": "My legalHold with sources",
    "description": "Created from Graph API",
    "contentQuery": "Bazooka",
    "userSources@odata.bind": [
        {
            "@odata.type": "microsoft.graph.security.userSource",
            "email": "SalesTeam@M365x809305.OnMicrosoft.com"
        }
    ],
    "siteSources@odata.bind": [
        {
            "@odata.type": "microsoft.graph.security.siteSource",
            "site": {
                "webUrl": "https://m365x809305.sharepoint.com/sites/Design-topsecret"
            }
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-ediscoveryholdpolicy-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-ediscoveryholdpolicy-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-ediscoveryholdpolicy-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-ediscoveryholdpolicy-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-ediscoveryholdpolicy-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryHoldPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/legalHolds/$entity",
    "isEnabled": true,
    "errors": [],
    "contentQuery": "Bazooka",
    "description": "Created from Graph API",
    "createdDateTime": "2022-05-23T03:54:11.1Z",
    "lastModifiedDateTime": "2022-05-23T03:54:11.1Z",
    "status": "pending",
    "id": "b9758bbc-ddbd-45e0-8484-3eb49cf1ded3",
    "displayName": "My legalHold with sources",
    "createdBy": {
        "application": null,
        "user": {
            "id": "MOD Administrator",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "user": {
            "id": "MOD Administrator",
            "displayName": null
        }
    }
}
```

