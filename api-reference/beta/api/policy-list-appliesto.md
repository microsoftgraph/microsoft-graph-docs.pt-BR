---
title: Lista de aplicativos e entidades de serviço com políticas específicas atribuídas
description: Recupere o aplicativo e objetos de entidades de serviço com a diretiva especificada atribuída.
localization_priority: Normal
ms.openlocfilehash: 21a5a9ba4260e306553f53866657a482d814b5f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875604"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>Lista de aplicativos e entidades de serviço com políticas específicas atribuídas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Recupere os objetos de [aplicativo](../resources/application.md) e [serviço principal](../resources/serviceprincipal.md) com a diretiva especificada atribuída.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

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

Se tiver êxito, este método retornará `200 OK` objetos de código e o [aplicativo](../resources/application.md) e a [entidade de serviço](../resources/serviceprincipal.md) de resposta no corpo da resposta. Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.

## <a name="example"></a>Exemplo
O exemplo a seguir recupera os aplicativos e entidades de serviço com uma diretiva específica atribuída.

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
