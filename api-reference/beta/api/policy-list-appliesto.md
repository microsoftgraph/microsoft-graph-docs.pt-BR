---
title: Listar aplicativos e entidades de serviço com política específica atribuída
description: Obter os objetos de entidade de serviço e aplicativo com a política especificada atribuída.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7959f8b286f1068de454f6d0d36a182f190efafd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455519"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>Listar aplicativos e entidades de serviço com política específica atribuída

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter os objetos de [entidade de serviço](../resources/serviceprincipal.md) e [aplicativo](../resources/application.md) com a política especificada atribuída.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="example"></a>Exemplo
O exemplo a seguir recupera os aplicativos e entidades de serviço com uma política específica atribuída.

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
