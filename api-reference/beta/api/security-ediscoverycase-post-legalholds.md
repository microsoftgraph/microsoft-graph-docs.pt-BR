---
title: Criar ediscoveryHoldPolicy
description: Crie um novo objeto ediscoveryHoldPolicy.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6746161f8a5562c56a51c8e301b23734fadb243c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945254"
---
# <a name="create-ediscoveryholdpolicy"></a>Criar ediscoveryHoldPolicy
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
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
|description|Cadeia de caracteres|A descrição da política de retenção legal. Opcional.|
|contentQuery|String|A consulta de conteúdo da política de retenção legal. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta [e um objeto ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
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
### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
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

