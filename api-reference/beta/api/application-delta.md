---
title: 'aplicativo: delta'
description: Get recentemente criado, atualizado ou excluído aplicativos sem precisar realizar uma leitura completa do conjunto de recurso inteiro. Consulte usando Delta consulta para obter detalhes.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4479048865d50cb0887d938708cb44ff62a4a9b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917192"
---
# <a name="application-delta"></a>aplicativo: delta

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Get recentemente criado, atualizado ou excluído aplicativos sem precisar realizar uma leitura completa do conjunto de recurso inteiro. Consulte [Usando Delta consulta](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.ReadWrite.All, Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar alterações, você deve fazer uma solicitação, incluindo a função delta no recurso de aplicativo. 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a>Parâmetros de consulta

Controle de alterações provoca uma round de um ou mais chamadas de função **delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** . O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornados no `deltaLink` URL da chamada de função **delta** anterior para o mesmo conjunto de recursos, indicando a conclusão do que round de controle de alterações. Salvar e aplicar a toda a `deltaLink` URL incluindo este token na primeira solicitação da próxima fase de rastreamento para esse conjunto de alterações.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornados no `nextLink` URL da chamada de função **delta** anterior, indicando que não há mais alterações a serem rastreados no mesmo conjunto de recursos. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 

- Não há suporte limitado para `$filter`:
  * A única suportada `$filter` expression é para controle de alterações de recursos específicos, por sua id: `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`. O número de identificações, que você pode especificar é limitado pelo comprimento máximo da URL.


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` objeto de coleção códigos e [aplicativos](../resources/application.md) de resposta no corpo da resposta. A resposta também inclui uma URL de nextLink ou uma URL de deltaLink. 

- Se um `nextLink` URL é retornado, existem páginas adicionais de dados a ser recuperado na sessão. O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.

- Se um `deltaLink` URL é retornado, não há nenhum dado mais sobre o estado existente do recurso a ser retornado. Persistir e usar o `deltaLink` URL para saber mais sobre as alterações do recurso no futuro.

Confira:</br>
- [Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</br>
- [Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</br>

### <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a>Resposta
Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
