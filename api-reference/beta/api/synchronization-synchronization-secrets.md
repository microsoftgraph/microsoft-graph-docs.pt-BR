---
title: 'sincronização: segredos'
description: Forneça credenciais para estabelecer conectividade com o sistema de destino.
ms.localizationpriority: medium
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 955dc53dcefb499fd3fe8e75e30dc1509d396629
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348758"
---
# <a name="synchronization-secrets"></a>sincronização: segredos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Forneça credenciais para estabelecer conectividade com o sistema de destino.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     |Directory.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |Sem suporte. |
|Aplicativo                            |Application.ReadWrite.OwnedBy, Directory.ReadWrite.All | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/secrets
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|credenciais|[coleção synchronizationSecretKeyStringValuePair](../resources/synchronization-synchronizationsecretkeystringvaluepair.md)|Credenciais para validar. Ignorado quando o **parâmetro useSavedCredentials** for `true`.|

## <a name="response"></a>Resposta
Se os segredos são salvos com êxito, este método retorna um código `204 No Content` de resposta. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronization_secrets"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets
Content-type: application/json

{
    "value": [
        {
            "key": "BaseAddress",
            "value": "user@domain.com"
        },
        {
            "key": "SecretToken",
            "value": "password-value"
        },
        {
            "key": "SyncNotificationSettings",
            "value": "{\"Enabled\":false,\"DeleteThresholdEnabled\":false}"
        },
        {
            "key": "SyncAll",
            "value": "false"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-secrets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-secrets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-secrets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronization: secrets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
