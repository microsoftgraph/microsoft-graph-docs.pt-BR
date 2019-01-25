---
title: Política de atualização
description: Atualize propriedades em uma diretiva preexistente.
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515409"
---
# <a name="update-policy"></a>Política de atualização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize propriedades em uma [política](../resources/policy.md)de preexistente.

## <a name="permissions"></a>Permissões
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
|Definição|String|A versão stringified do objeto de [diretiva](../resources/policy.md) .|
|displayName|String|Um nome personalizado para a política.|
|isOrganizationDefault|Booliano|Especifica se esta política é aplicada por padrão.|
|type|String|Especifica o tipo de política. No momento deve ser "TokenLifetimePolicy"|

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
