---
title: Política de atualização
description: Atualize propriedades em uma diretiva preexistente.
localization_priority: Normal
ms.openlocfilehash: 2992f2f76c0e8b213ad8aabca1bfd0fe59883989
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857152"
---
# <a name="update-policy"></a>Política de atualização

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atualize propriedades em uma [política](../resources/policy.md)de preexistente.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | application/json  | Natureza dos dados no corpo de uma entidade. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornecem um objeto JSON com os parâmetros que precisam ser atualizados. A tabela a seguir mostra os parâmetros possíveis.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definição|Cadeia de caracteres|A versão stringified do objeto de [diretiva](../resources/policy.md) .|
|displayName|Cadeia de caracteres|Um nome personalizado para a política.|
|isOrganizationDefault|Booliano|Especifica se esta política é aplicada por padrão.|
|type|Cadeia de caracteres|Especifica o tipo de política. No momento deve ser "TokenLifetimePolicy"|

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `204 No Content`. Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.

## <a name="example"></a>Exemplo
O exemplo a seguir atualiza a definição da diretiva de vida útil do token e define como o padrão da organização.

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 204 No Content
```
