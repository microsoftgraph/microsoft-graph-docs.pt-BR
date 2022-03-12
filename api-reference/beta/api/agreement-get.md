---
title: Obter contrato
description: Recupere as propriedades e as relações de um objeto de contrato.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 1733714cd3ef6f971caefa204c14f73bde82605d
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451358"
---
# <a name="get-agreement"></a>Obter contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um [objeto de](../resources/agreement.md) contrato.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Agreement.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório. Para saber mais sobre funções de diretório, consulte [Funções in-loco do Azure AD](/azure/active-directory/roles/permissions-reference):
+ Administrador Global
+ Administrador de Acesso Condicional
+ Administrador de Segurança

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao parâmetro `$select` [de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta [e um objeto agreement](../resources/agreement.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-an-agreement"></a>Exemplo 1: Recuperar um contrato

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/0ec9f6a6-159d-4dd8-a563-1f0b5935e80b
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#agreements/$entity",
    "id": "0ec9f6a6-159d-4dd8-a563-1f0b5935e80b",
    "displayName": "All users terms of use",
    "termsExpiration": null,
    "userReacceptRequiredFrequency": "P90D",
    "isViewingBeforeAcceptanceRequired": false,
    "isPerDeviceAcceptanceRequired": false
}
```


### <a name="example-2-retrieve-an-agreement-and-its-related-files"></a>Exemplo 2: recuperar um contrato e seus arquivos relacionados

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_agreement_files"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be?$expand=files
```


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#agreements(files())/$entity",
    "id": "0ec9f6a6-159d-4dd8-a563-1f0b5935e80b",
    "displayName": "All users terms of use",
    "termsExpiration": null,
    "userReacceptRequiredFrequency": "P90D",
    "isViewingBeforeAcceptanceRequired": false,
    "isPerDeviceAcceptanceRequired": false,
    "files@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/termsOfUse/agreements('0ec9f6a6-159d-4dd8-a563-1f0b5935e80b')/files",
    "files": [
        {
            "id": "681b73a7-e9ae-4f2d-aca5-9e857599cd15",
            "fileName": "ToU.pdf",
            "displayName": "Contoso Terms of Use",
            "language": "en-GB",
            "isDefault": true,
            "isMajorVersion": false,
            "createdDateTime": "2022-03-02T14:11:32.885186Z",
            "fileData": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
