---
title: Atribuir política
description: Atribui uma política a um aplicativo ou a uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f005973677ca3e430706a7fced22e5fbf51bcd0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455531"
---
# <a name="assign-policy"></a>Atribuir política

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atribui uma [política](../resources/policy.md) a um aplicativo ou a uma entidade de serviço.

>Observação: no momento, a atribuição de política se aplica apenas à política de tempo de vida do token. Esse tipo de política é descrita na [política](../resources/policy.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> Observação: "ID" na solicitação é a propriedade "ID" da entidade de serviço ou aplicativo, não a propriedade "AppID".

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | application/json  | Natureza dos dados no corpo de uma entidade. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto Policy a ser adicionado.

## <a name="response"></a>Resposta

Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="example"></a>Exemplo
O exemplo a seguir atribui uma política a um aplicativo.

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 204 No Content
```
