---
title: Obter as alterações incrementais para grupos
description: Use a consulta delta para descobrir alterações sem buscar todo o conjunto de grupos para comparar as alterações. O exemplo a seguir mostra uma série de solicitações para controlar alterações em grupos.
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: c4cdd00fac6be32f4a4338116ce47cb63d1723a4
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668892"
---
# <a name="get-incremental-changes-for-groups"></a>Obter as alterações incrementais para grupos

A [consulta delta](./delta-query-overview.md) no Microsoft Graph permite consultar adições, exclusões ou atualizações de [recursos com suporte](delta-query-overview.md#supported-resources). Ele é habilitado por meio de uma série de [delta](/graph/api/group-delta?) solicitações. Para grupos, a consulta delta permite que você descubra alterações sem buscar todo o conjunto de grupos para comparar as alterações.

Os clientes que sincronizam grupos com um repositório de perfil local podem utilizar a consulta delta para a sincronização inicial completa, juntamente com as sincronizações incremental subsequentes. Normalmente, um cliente faria uma sincronização completa inicial de todos os grupos em um locatário e, em seguida, obteria alterações incrementais para grupos periodicamente.

## <a name="track-changes-to-groups"></a>Controlar alterações em grupos

Acompanhe as alterações de grupos por meio de uma ou mais solicitações GET com função **delta**. A solicitação GET é como uma solicitação de [grupos de lista](/graph/api/group-list?), exceto com os seguintes objetos extras na URL:

- A função **delta**.
- Um [token de estado](./delta-query-overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.

## <a name="example-track-changes-to-groups"></a>Exemplo para controlar alterações em grupos

O exemplo a seguir mostra uma série de solicitações para controlar alterações em grupos:

1. Uma [solicitação inicial](#initial-request) e [réplica](#initial-response)
2. Uma [solicitação do nextLink](#nextlink-request) e [réplica](#nextlink-response)
3. Uma [final da solicitação nextLink](#final-nextlink-request) e [réplica](#final-nextlink-response)
4. Uma [solicitação de deltaLink](#deltalink-request) e [réplica de deltaLink](#deltalink-response)

Anote o seguinte nas respostas:

- Quando um grupo é excluído (Microsoft 365 grupos), o item contém uma anotação: `@removed` com valor de `"reason": "changed"`.
- Quando o grupo é excluído permanentemente (um grupo de segurança ou [excluindo permanentemente um grupo Microsoft 365](/graph/api/directory-deleteditems-list.)), o item contém uma anotação: `@removed` com valor de `"reason": "deleted"`.
- Quando o grupo é criado ou restaurado, não há anotação.

### <a name="initial-request"></a>Solicitação inicial

Para acompanhar as alterações no recurso de grupo, faça uma solicitação e inclua a função **delta** como um segmento de URL.

Anote os seguintes itens:

- O parâmetro de consulta `$select` opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.
- O parâmetro de consulta `$select` opcional também é usado para mostrar como os membros do grupo podem ser recuperados em conjunto com objetos de grupo. Isso permite o controle de alterações de associação, como quando usuários são adicionados ou removidos de grupos.
- A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados em solicitações subsequentes.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

### <a name="initial-response"></a>Resposta inicial

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](/graph/api/resources/group) no corpo da resposta. Se o conjunto de grupos inteiro for muito grande para caber em uma resposta, um `@odata.nextLink` contendo um token de estado também será incluído.

Neste exemplo, um `@odata.nextLink` foi incluído; o parâmetro de consulta `$select` original é codificado no token de estado.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"All Company",
      "description":"This is the default group for everyone in the network",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
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
    },
    {
      "displayName":"sg-HR",
      "description":"All HR personnel",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

> [!NOTE]
> A `members@delta`propriedade está incluída no primeiro objeto de grupo - **Toda a empresa** - e contém os dois membros atuais do grupo. **sg-HR** não contém essa propriedade porque o grupo não tem membros.

### <a name="nextlink-request"></a>solicitação nextLink

A segunda solicitação usa o `@odata.nextLink` da resposta anterior, que contém o `skipToken`. Observe que o parâmetro `$select` não está visivelmente presente, pois está codificado e incluído no token.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

### <a name="nextlink-response"></a>Resposta nextLink

A resposta contém outro `@odata.nextLink` com um novo valor `skipToken`, o que indica que mais alterações controladas para grupos estão disponíveis. Use a URL `@odata.nextLink` em mais solicitações até que uma URL de `@odata.deltaLink` (em um parâmetro `@odata.deltaLink`) seja retornada na resposta final, mesmo que o valor seja uma matriz vazia.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mark 8 Project Team",
      "description":"Mark 8 Project Team",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"Sales and Marketing",
      "description":"Sales and Marketing",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
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

### <a name="final-nextlink-request"></a>Solicitação nextLink final

A terceira solicitação usa a última `@odata.nextLink` retornada da última solicitação de sincronização.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>Resposta nextLink final

Quando um URL `@odata.deltaLink` é retornado, não há mais dados sobre o estado existente dos objetos de grupo.  Para solicitações futuras, o aplicativo utiliza o URL `@odata.deltaLink` para saber mais sobre outras alterações nos grupos. Salve o `deltaToken` e use-o no URL da solicitação subsequente para descobrir mais alterações nos grupos.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"All Employees",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"Remote living",
      "description":"Remote living",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

### <a name="deltalink-request"></a>Solicitação deltaLink

Usando a `@odata.deltaLink` da [última réplica](#final-nextlink-response), você receberá alterações (adições, exclusões ou atualizações) nos grupos desde a última solicitação. As alterações incluem:

- Objetos de grupo recém-criados.
- Objetos de grupo excluídos.
- Objetos de grupo para os quais uma propriedade foi alterada (por exemplo, **displayName** foi modificado).
- Objetos de grupo cujos objetos de membro foram adicionados ou removidos.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

### <a name="deltalink-response"></a>Resposta deltaLink

Se nenhuma alteração tiver ocorrido, um `@odata.deltaLink` será retornado sem resultados - o **valor** propriedade é uma matriz vazia. Substitua o link anterior no aplicativo pelo novo para usar em chamadas futuras.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Se houver alterações, um conjunto de grupos alterados será incluído. A resposta também contém um `@odata.nextLink`, caso haja várias páginas de alterações a serem recuperadas, ou um `@odata.deltaLink`. Implemente o mesmo padrão de seguir o `@odata.nextLink` e persistir o `@odata.deltaLink` final para chamadas futuras.

> [!NOTE]
> Essa solicitação pode ter atrasos de replicação para grupos que foram criados, atualizados ou excluídos recentemente. Repita `@odata.nextLink` ou `@odata.deltaLink` depois de algum tempo para recuperar as alterações mais recentes.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

Alguns aspectos a observar sobre a resposta do exemplo acima:

- Os objetos são retornados com o mesmo conjunto de propriedades originalmente especificado pelo parâmetro de consulta `$select`.

- As propriedades alteradas e inalteradas estão incluídas. No exemplo acima, a propriedade `description` tem um novo valor, enquanto a propriedade `displayName` não foi alterada.

- `members@delta` contém as seguintes alterações na associação de grupo.

  - O primeiro usuário da lista foi removido do grupo. Isso foi feito por meio da remoção da associação ou exclusão do objeto de usuário. A propriedade `@removed` descreve esse procedimento. Somente os usuários que tiverem sido excluídos permanentemente serão removidos dos grupos. Os usuários que foram excluídos temporariamente mantêm suas associações de grupo e não aparecerão no resultado delta até que sejam excluídos permanentemente. Para obter mais detalhes, consulte [diretório (itens deletados)](/graph/api/resources/directory).

  - O segundo usuário foi adicionado ao grupo.

## <a name="paging-through-members-in-a-large-group"></a>Ver membros de um grande grupo

A propriedade `members@delta` é incluída em objetos de grupo por padrão, quando o parâmetro de consulta `$select` não foi especificado ou quando o parâmetro `$select=members` é especificado explicitamente. Para grupos com muitos membros, é possível que todos os membros não caibam em uma única resposta. Implemente o padrão a seguir para lidar com esses casos.

> [!NOTE]
> Esse padrão aplica-se à recuperação inicial do estado de grupo e às chamadas subsequentes para obter as alterações da consulta delta.

Vamos supor que você esteja executando a seguinte consulta delta– para capturar o estado completo inicial dos grupos ou posteriormente para obter alterações delta:

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

1. O Microsoft Graph pode retornar uma resposta com apenas um objeto de grupo, com uma lista grande de membros na propriedade `members@delta`:

**Primeira página**

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. Ao seguir o `@odata.nextLink`, você poderá receber uma resposta contendo o mesmo objeto de grupo. Os mesmos valores de propriedade serão retornados, mas a propriedade `members@delta` agora contém uma lista de usuários diferente.

**Segunda página**

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. A lista de membros completa será retornada dessa maneira, e outros grupos começarão a aparecer na resposta.

As seguintes práticas recomendadas devem ser seguidas para lidar corretamente com esse padrão:
- Siga sempre o `@odata.nextLink` e mescle localmente o estado de cada grupo. Quando receber respostas relacionadas ao mesmo grupo, use-as para criar a lista completa de associação no aplicativo.
- Não suponha uma sequência específica das respostas. Suponha que o mesmo grupo possa aparecer em qualquer lugar na sequência do `@odata.nextLink` e leve isso em conta na sua lógica de mesclagem.


## <a name="see-also"></a>Confira também
Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).
