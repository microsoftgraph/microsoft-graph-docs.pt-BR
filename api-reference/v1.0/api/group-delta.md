---
title: 'group: delta'
description: Obtenha grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação de grupo, sem precisar executar uma leitura completa de toda a coleção de grupos.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 00890d751a4b4a4ec9d66e89501c893446f33476
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203894"
---
# <a name="group-delta"></a>group: delta

Namespace: microsoft.graph

Obtenha grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação de grupo, sem precisar executar uma leitura completa de toda a coleção de grupos. Consulte [Usando a Consulta Delta para](/graph/delta-query-overview) obter detalhes.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                                         |
| Aplicativo                            | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.

Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.

Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta | Tipo   | Descrição                                                                                                                                                                                                                                                                                                                                                   |
| :-------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| $deltatoken     | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção. |
| $skiptoken      | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.                                                                                                                                                         |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Esse método dá suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.
- Você pode usar para `$select=members` obter alterações de associação. Além disso, você pode acompanhar outras alterações, como propriedade e muito mais, selecionando qualquer relação [de](../resources/group.md#relationships) grupo do tipo **coleção directoryObject**.
- Há suporte limitado para `$filter`:
  - A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`. É possível filtrar vários objetos. Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Há um limite de 50 objetos filtrados.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                                                                                                                                                                    |
| :------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autorização | &lt;Token&gt; de portador                                                                                                                                                           |
| Content-Type  | application/json                                                                                                                                                               |
| Preferir        | return=minimal <br><br>Especificar este cabeçalho com uma solicitação que utiliza um `deltaLink` retornaria apenas as propriedades do objeto que foram alteradas desde a última rodada. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta também inclui um token de estado que é uma `nextLink` URL ou uma `deltaLink` URL.

- Se uma URL `nextLink` for retornada:

  - Isso indica que há páginas adicionais de dados a serem recuperados na sessão. O aplicativo continua fazendo solicitações usando o URL `nextLink` até que um URL `deltaLink` seja incluído na resposta.
  - A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial. Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.

- Se uma URL `deltaLink` for retornada:
  - Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso. Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.
  - Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Padrão: retornar as mesmas propriedades de uma solicitação delta inicial

Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, o valor antigo será incluído na resposta.
- Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.

> **Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não. Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedade , conforme mostrado no [segundo exemplo abaixo](#request-2) .

#### <a name="alternative-return-only-the-changed-properties"></a>Alternativa: retornar somente as propriedades alteradas

Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma. (Diferente do comportamento padrão.)

> **Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta. O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada. Veja o [terceiro exemplo](#request-3) a seguir.

### <a name="example"></a>Exemplo

#### <a name="request-1"></a>Solicitação 1

Este é um exemplo de solicitação. Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a>Resposta 1

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
>
> Observe a presença da propriedade _members@delta_ que inclui as IDs de objetos membro no grupo.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "createdDateTime":"2021-03-12T10:36:14Z",
      "description":"This is the default group for everyone in the network",
      "displayName":"All Company",
      "groupTypes": [
        "Unified"
      ],
      "mail": "allcompany@contoso.com",
      "members@delta": [
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "693acd06-2877-4339-8ade-b704261fe7a0"
        },
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "49320844-be99-4164-8167-87ff5d047ace"
        }
      ]
    }
  ]
}
```

#### <a name="request-2"></a>Solicitação 2

O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações, com o comportamento de resposta padrão:

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_delta_with_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-with-select-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-with-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-with-select-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-with-select-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-2"></a>Resposta 2

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que `deltaLink` foi obtido.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "All Company",
      "description": null,
      "mailNickname": "allcompany@contoso.com"
    }
  ]
}
```

#### <a name="request-3"></a>Solicitação 3

O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa:

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-minimal-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-delta-minimal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-minimal-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-delta-minimal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-3"></a>Resposta 3

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que a propriedade `mailNickname` não foi incluída, ou seja, não foi alterada desde a última consulta delta; `displayName` e `description` foram incluídas, o que significa que os valores foram alterados.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Everyone",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).
- [Obter alterações incrementais para grupos](/graph/delta-query-groups).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
