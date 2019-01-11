---
title: Atribuir política
description: Atribui uma política a um aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 30ba92c1d0308f9c4846702008a203821ae2b7b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865454"
---
# <a name="assign-policy"></a>Atribuir política

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atribui uma [política](../resources/policy.md) a um aplicativo ou entidade de serviço.

>Observação: No momento, a atribuição da diretiva só se aplica a vida útil do Token política. Esse tipo de política é descrito na [política](../resources/policy.md).

## <a name="permissions"></a>Permissions
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

> Observação: O "id" na solicitação é a propriedade "id" do aplicativo ou serviço principal, não a propriedade "appid".

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | application/json  | Natureza dos dados no corpo de uma entidade. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornecem uma representação de JSON do objeto de diretiva a ser adicionado.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `204 No Content`. Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.

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
