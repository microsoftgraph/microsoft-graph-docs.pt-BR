---
title: Obter as alterações incrementais para grupos
description: A consulta delta permite consultar adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função delta. A consulta delta permite que você descubra alterações nos grupos
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 4fc09f8005e72480e6b716ebdacc6a7f0242a80ef4f01f2311205e32f0c1e6c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189139"
---
# <a name="get-incremental-changes-for-groups"></a>Obter as alterações incrementais para grupos

A [Consulta delta](./delta-query-overview.md) permite que você consulte adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função [delta](/graph/api/group-delta?view=graph-rest-1.0). A consulta Delta permite que você descubra alterações em grupos sem ter que buscar todo o conjunto de grupos do Microsoft Graph e comparar as alterações.

Clientes que sincronizam grupos com um repositório de perfil local, podem usar a Consulta Delta para a sincronização completa inicial juntamente com as sincronizações incrementais no futuro. Normalmente, um cliente faria uma sincronização completa inicial de todos os grupos em um locatário e, logo após, obteria alterações incrementais para esses grupos periodicamente.

## <a name="tracking-group-changes"></a>Controle de alterações de grupo

O controle de alterações de grupo corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar grupos](/graph/api/group-list?view=graph-rest-1.0), exceto se você incluir o seguinte:

- A função **delta**.
- Um [token de estado](./delta-query-overview.md) (*deltaToken* ou *skipToken*) da chamada de função GET **delta** anterior.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos grupos:

1. [Solicitação inicial](#initial-request) e [resposta](#initial-response)
2. [solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)
3. [Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)
4. [Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)

## <a name="initial-request"></a>Solicitação inicial

Para iniciar o rastreamento de alterações no recurso de grupo, faça uma solicitação incluindo a função delta no recurso de grupo.

Observe o seguinte:

- O parâmetro de consulta `$select` opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.
- O parâmetro de consulta `$select` opcional também é usado para mostrar como os membros do grupo podem ser recuperados em conjunto com objetos de grupo. Isso permite o controle de alterações de associação, como quando usuários são adicionados ou removidos de grupos.
- A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

## <a name="initial-response"></a>Resposta inicial

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](/graph/api/resources/group?view=graph-rest-1.0) no corpo da resposta. Se o conjunto de grupos inteiro for muito grande para caber em uma resposta, um `nextLink` contendo um token de estado também será incluído.

Neste exemplo, um `nextLink` foi incluído; o parâmetro de consulta `$select` original é codificado no token de estado.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
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
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**Observação:** a propriedade `members@delta` está incluída no primeiro objeto de grupo, o TestGroup1, e contém os dois membros atuais do grupo. O TestGroup2 não contém essa propriedade porque o grupo não tem nenhum membro.

## <a name="nextlink-request"></a>solicitação nextLink

A segunda solicitação usa o `nextLink` da resposta anterior, que contém o `skipToken`. Observe que o parâmetro `$select` não está presente explicitamente porque ele é codificado no token.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>Resposta nextLink

A resposta contém outro `nextLink` com outro valor de `skipToken`, indicando que há mais grupos disponíveis. Você deve continuar criando solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja retornada na resposta final, mesmo que o valor seja uma matriz vazia (isso pode ocorrer em determinadas circunstâncias).

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
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

## <a name="final-nextlink-request"></a>Solicitação nextLink final

A terceira solicitação novamente usa o `nextLink` mais recente.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Resposta nextLink final

Por fim, a URL `deltaLink` é retornada, o que significa que não há mais dados para o estado de grupos existente. Para solicitações futuras, o aplicativo usa o `deltaLink` e o valor de `deltaToken` que contém para saber mais sobre novas alterações nos grupos.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>Solicitação deltaLink

Usando o `deltaLink` da [última resposta](#final-nextlink-response), é possível obter as novas alterações de rede do grupo desde a última solicitação. As alterações incluem:
- Objetos de grupo recém-criados.
- Objetos de grupo excluídos.
- Objetos de grupo cuja propriedade mudou (por exemplo, **displayName** foi modificada).
- Objetos de grupo cujos objetos de membro foram adicionados ou removidos.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>Resposta deltaLink

Se não houver alterações, um `deltaLink` será retornado sem resultados. A propriedade `value` fica em branco. Substitua o link anterior no aplicativo pelo novo para usar em chamadas futuras.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Se houver alterações, um conjunto de grupos alterados será incluído. A resposta também contém um `nextLink`, caso haja várias páginas de alterações a serem recuperadas, ou um `deltaLink`. Implemente o mesmo padrão, seguindo os `nextLinks`, como antes, e mantenha o `deltaLink` final para chamadas futuras.

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

- Propriedades alteradas e inalteradas estão incluídas. No exemplo acima, a propriedade `description` tem um novo valor, e a propriedade `displayName` não foi alterada.

- `members@delta` contém todas as alterações de associação.

  - O primeiro usuário da lista foi removido do grupo. Isso foi feito por meio da remoção da associação ou exclusão do objeto de usuário. A propriedade `@removed` descreve esse procedimento. Somente os usuários que tiverem sido excluídos permanentemente serão removidos dos grupos. Os usuários que foram excluídos temporariamente mantêm suas participações no grupo e não serão exibidos no resultado delta até que tenham sido excluídos permanentemente. Para obter mais detalhes, consulte [diretório (itens deletados)](/graph/api/resources/directory?view=graph-rest-1.0).

  - O segundo usuário foi adicionado ao grupo.

## <a name="paging-through-members-in-a-large-group"></a>Ver membros de um grande grupo

A propriedade `members@delta` é incluída em objetos de grupo por padrão quando o parâmetro de consulta `$select` não foi especificado ou quando o parâmetro `$select=members` é explicitamente especificado. No caso de grupos com muitos membros, é possível que nem todos caibam em uma resposta única. Nesta seção, descrevemos o padrão a ser implementado para lidar com essas situações.

>**Observação:** esse padrão aplica-se à recuperação inicial do estado de grupo e às chamadas subsequentes para obter as alterações da consulta delta.

Vamos supor que você esteja executando a consulta delta a seguir para capturar o estado inicial completo de grupos ou posteriormente para obter alterações da consulta delta:

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

2. Quando você seguir o `nextLink`, poderá receber uma resposta novamente com o mesmo objeto de grupo. Os mesmos valores de propriedade serão retornados, mas a propriedade `members@delta` agora contém uma lista de usuários diferente.

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
- Siga sempre o `nextLink` e mescle localmente o estado de cada grupo. Quando receber respostas relacionadas ao mesmo grupo, use-as para criar a lista completa de associação no aplicativo.
- É aconselhável não presumir uma sequência específica de respostas. Suponha que o mesmo grupo possa aparecer em qualquer lugar na sequência do `nextLink` e leve isso em conta na sua lógica de mesclagem.


## <a name="see-also"></a>Confira também
Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).
