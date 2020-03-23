---
title: Obter as alterações incrementais para grupos
description: A consulta delta permite que você consulte adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função delta. A consulta delta permite que você descubra as alterações nos grupos
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 0f91b33218ad07d140b910e061bdf3a76d676573
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892657"
---
# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="9734e-104">Obter as alterações incrementais para grupos</span><span class="sxs-lookup"><span data-stu-id="9734e-104">Get incremental changes for groups</span></span>

<span data-ttu-id="9734e-p102">A [Consulta delta](./delta-query-overview.md) permite que você consulte adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função [delta](/graph/api/group-delta?view=graph-rest-1.0). A consulta Delta permite que você descubra alterações em grupos sem ter que buscar todo o conjunto de grupos do Microsoft Graph e comparar as alterações.</span><span class="sxs-lookup"><span data-stu-id="9734e-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](/graph/api/group-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="9734e-p103">Clientes que sincronizam grupos com um repositório de perfil local, podem usar a Consulta Delta para a sincronização completa inicial juntamente com as sincronizações incrementais no futuro. Normalmente, um cliente faria uma sincronização completa inicial de todos os grupos em um locatário e, logo após, obteria alterações incrementais para esses grupos periodicamente.</span><span class="sxs-lookup"><span data-stu-id="9734e-p103">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span>

## <a name="tracking-group-changes"></a><span data-ttu-id="9734e-109">Controle de alterações de grupo</span><span class="sxs-lookup"><span data-stu-id="9734e-109">Tracking group changes</span></span>

<span data-ttu-id="9734e-p104">O controle de alterações de grupo corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar grupos](/graph/api/group-list?view=graph-rest-1.0), exceto se você incluir o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9734e-p104">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](/graph/api/group-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="9734e-112">A função **delta**.</span><span class="sxs-lookup"><span data-stu-id="9734e-112">The **delta** function.</span></span>
- <span data-ttu-id="9734e-113">Um [token de estado](./delta-query-overview.md) (*deltaToken* ou *skipToken*) da chamada de função GET **delta** anterior.</span><span class="sxs-lookup"><span data-stu-id="9734e-113">A [state token](./delta-query-overview.md) (*deltaToken* or *skipToken*) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="9734e-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9734e-114">Example</span></span>

<span data-ttu-id="9734e-115">O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos grupos:</span><span class="sxs-lookup"><span data-stu-id="9734e-115">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="9734e-116">[Solicitação inicial](#initial-request) e [resposta](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="9734e-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="9734e-117">[solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="9734e-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="9734e-118">[Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="9734e-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="9734e-119">[Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="9734e-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="9734e-120">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="9734e-120">Initial request</span></span>

<span data-ttu-id="9734e-121">Para iniciar o rastreamento de alterações no recurso de grupo, faça uma solicitação incluindo a função delta no recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="9734e-121">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span>

<span data-ttu-id="9734e-122">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9734e-122">Note the following:</span></span>

- <span data-ttu-id="9734e-123">O parâmetro de consulta `$select` opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.</span><span class="sxs-lookup"><span data-stu-id="9734e-123">The optional `$select` query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="9734e-124">O parâmetro de consulta `$select` opcional também é usado para mostrar como os membros do grupo podem ser recuperados em conjunto com objetos de grupo.</span><span class="sxs-lookup"><span data-stu-id="9734e-124">The optional `$select` query parameter is also used to show how group members can be retrieved together with group objects.</span></span> <span data-ttu-id="9734e-125">Isso permite o controle de alterações de associação, como quando usuários são adicionados ou removidos de grupos.</span><span class="sxs-lookup"><span data-stu-id="9734e-125">This allows tracking of membership changes, such as when users are added or removed from groups.</span></span>
- <span data-ttu-id="9734e-p106">A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="9734e-p106">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

## <a name="initial-response"></a><span data-ttu-id="9734e-128">Resposta inicial</span><span class="sxs-lookup"><span data-stu-id="9734e-128">Initial response</span></span>

<span data-ttu-id="9734e-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](/graph/api/resources/group?view=graph-rest-1.0) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9734e-129">If successful, this method returns `200 OK` response code and [group](/graph/api/resources/group?view=graph-rest-1.0) collection object in the response body.</span></span> <span data-ttu-id="9734e-130">Se o conjunto de grupos inteiro for muito grande para caber em uma resposta, um `nextLink` contendo um token de estado também será incluído.</span><span class="sxs-lookup"><span data-stu-id="9734e-130">If the entire set of groups is too large to fit in one response, a `nextLink` containing a state token will also be included.</span></span>

<span data-ttu-id="9734e-131">Neste exemplo, um `nextLink` foi incluído; o parâmetro de consulta `$select` original é codificado no token de estado.</span><span class="sxs-lookup"><span data-stu-id="9734e-131">In this example, a `nextLink` was included; the original `$select` query parameter is encoded in the state token.</span></span>

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

><span data-ttu-id="9734e-132">**Observação:**  a propriedade `members@delta` está incluída no primeiro objeto de grupo, o TestGroup1, e contém os dois membros atuais do grupo.</span><span class="sxs-lookup"><span data-stu-id="9734e-132">**Note:** The `members@delta` property is included in the first group object - TestGroup1 - and contains the two current members of the group.</span></span> <span data-ttu-id="9734e-133">O TestGroup2 não contém essa propriedade porque o grupo não tem nenhum membro.</span><span class="sxs-lookup"><span data-stu-id="9734e-133">TestGroup2 does not contain that property because the group does not have any members.</span></span>

## <a name="nextlink-request"></a><span data-ttu-id="9734e-134">solicitação nextLink</span><span class="sxs-lookup"><span data-stu-id="9734e-134">nextLink request</span></span>

<span data-ttu-id="9734e-135">A segunda solicitação usa o `nextLink` da resposta anterior, que contém o `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="9734e-135">The second request uses the `nextLink` from the previous response, which contains the `skipToken`.</span></span> <span data-ttu-id="9734e-136">Observe que o parâmetro `$select` não está presente explicitamente porque ele é codificado no token.</span><span class="sxs-lookup"><span data-stu-id="9734e-136">Notice the `$select` parameter is not explicitly present as it is encoded in the token.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="9734e-137">Resposta nextLink</span><span class="sxs-lookup"><span data-stu-id="9734e-137">nextLink response</span></span>

<span data-ttu-id="9734e-138">A resposta contém outro `nextLink` com outro valor de `skipToken`, indicando que há mais grupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9734e-138">The response contains another `nextLink` with a new `skipToken` value, which indicates that more groups are available.</span></span> <span data-ttu-id="9734e-139">Você deve continuar criando solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja retornada na resposta final, mesmo que o valor seja uma matriz vazia (isso pode ocorrer em determinadas circunstâncias).</span><span class="sxs-lookup"><span data-stu-id="9734e-139">You should continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response, even if the value is an empty array (this can happen under certain circumstances).</span></span>

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

## <a name="final-nextlink-request"></a><span data-ttu-id="9734e-140">Solicitação nextLink final</span><span class="sxs-lookup"><span data-stu-id="9734e-140">Final nextLink request</span></span>

<span data-ttu-id="9734e-141">A terceira solicitação novamente usa o `nextLink` mais recente.</span><span class="sxs-lookup"><span data-stu-id="9734e-141">The third request again uses the latest `nextLink`.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="9734e-142">Resposta nextLink final</span><span class="sxs-lookup"><span data-stu-id="9734e-142">Final nextLink response</span></span>

<span data-ttu-id="9734e-143">Por fim, a URL `deltaLink` é retornada, o que significa que não há mais dados para o estado de grupos existente.</span><span class="sxs-lookup"><span data-stu-id="9734e-143">Finally, the `deltaLink` URL is returned, which means there is no more data for the existing state of groups.</span></span> <span data-ttu-id="9734e-144">Para solicitações futuras, o aplicativo usa o `deltaLink` e o valor de `deltaToken` que contém para saber mais sobre novas alterações nos grupos.</span><span class="sxs-lookup"><span data-stu-id="9734e-144">For future requests, the application uses the `deltaLink` and the `deltaToken` value it contains to learn about new changes to groups.</span></span>

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

## <a name="deltalink-request"></a><span data-ttu-id="9734e-145">Solicitação deltaLink</span><span class="sxs-lookup"><span data-stu-id="9734e-145">deltaLink request</span></span>

<span data-ttu-id="9734e-146">Usando o `deltaLink` da [última resposta](#final-nextlink-response), é possível obter as novas alterações de rede do grupo desde a última solicitação.</span><span class="sxs-lookup"><span data-stu-id="9734e-146">Using the `deltaLink` from the [last response](#final-nextlink-response), you will be able to get net new changes to groups since the last request.</span></span> <span data-ttu-id="9734e-147">As alterações incluem:</span><span class="sxs-lookup"><span data-stu-id="9734e-147">Changes include:</span></span>
- <span data-ttu-id="9734e-148">Objetos de grupo recém-criados.</span><span class="sxs-lookup"><span data-stu-id="9734e-148">Newly created group objects.</span></span>
- <span data-ttu-id="9734e-149">Objetos de grupo excluídos.</span><span class="sxs-lookup"><span data-stu-id="9734e-149">Deleted group objects.</span></span>
- <span data-ttu-id="9734e-150">Objetos de grupo cuja propriedade mudou (por exemplo, **displayName** foi modificada).</span><span class="sxs-lookup"><span data-stu-id="9734e-150">Group objects for which a property has changed (e.g. **displayName** has been modified).</span></span>
- <span data-ttu-id="9734e-151">Objetos de grupo cujos objetos de membro foram adicionados ou removidos.</span><span class="sxs-lookup"><span data-stu-id="9734e-151">Group objects for which member objects have been added or removed.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="9734e-152">Resposta deltaLink</span><span class="sxs-lookup"><span data-stu-id="9734e-152">deltaLink response</span></span>

<span data-ttu-id="9734e-153">Se não houver alterações, um `deltaLink` será retornado sem resultados. A propriedade `value` fica em branco.</span><span class="sxs-lookup"><span data-stu-id="9734e-153">If no changes have occurred, a `deltaLink` is returned with no results - the `value` property is empty.</span></span> <span data-ttu-id="9734e-154">Substitua o link anterior no aplicativo pelo novo para usar em chamadas futuras.</span><span class="sxs-lookup"><span data-stu-id="9734e-154">Make sure to replace the previous link in the application with the new one for use in future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="9734e-155">Se houver alterações, um conjunto de grupos alterados será incluído.</span><span class="sxs-lookup"><span data-stu-id="9734e-155">If changes have occurred, a collection of changed groups is included.</span></span> <span data-ttu-id="9734e-156">A resposta também contém um `nextLink`, caso haja várias páginas de alterações a serem recuperadas, ou um `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="9734e-156">The response also contains either a `nextLink` - in case there are multiple pages of changes to retrieve - or a `deltaLink`.</span></span> <span data-ttu-id="9734e-157">Implemente o mesmo padrão, seguindo os `nextLinks`, como antes, e mantenha o `deltaLink` final para chamadas futuras.</span><span class="sxs-lookup"><span data-stu-id="9734e-157">You should implement the same pattern of following the `nextLinks` as before and persist the final `deltaLink` for future calls.</span></span>

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

<span data-ttu-id="9734e-158">Alguns aspectos a observar sobre a resposta do exemplo acima:</span><span class="sxs-lookup"><span data-stu-id="9734e-158">Some things to note about the example response above:</span></span>

- <span data-ttu-id="9734e-159">Os objetos são retornados com o mesmo conjunto de propriedades originalmente especificado pelo parâmetro de consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="9734e-159">The objects are returned with the same set of properties originally specified via the `$select` query parameter.</span></span>

- <span data-ttu-id="9734e-160">Propriedades alteradas e inalteradas estão incluídas.</span><span class="sxs-lookup"><span data-stu-id="9734e-160">Both changed and unchanged properties are included.</span></span> <span data-ttu-id="9734e-161">No exemplo acima, a propriedade `description` tem um novo valor, e a propriedade `displayName` não foi alterada.</span><span class="sxs-lookup"><span data-stu-id="9734e-161">In the example above, the `description` property has a new value, while the `displayName` property has not changed.</span></span>

- <span data-ttu-id="9734e-162">`members@delta` contém todas as alterações de associação.</span><span class="sxs-lookup"><span data-stu-id="9734e-162">`members@delta` contains any changes to membership.</span></span>

  - <span data-ttu-id="9734e-163">O primeiro usuário da lista foi removido do grupo. Isso foi feito por meio da remoção da associação ou exclusão do objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="9734e-163">The first user in the list has been removed from the group - either by removing the membership or by deleting the user object itself.</span></span> <span data-ttu-id="9734e-164">A propriedade `@removed` descreve esse procedimento.</span><span class="sxs-lookup"><span data-stu-id="9734e-164">The `@removed` property describes that.</span></span> <span data-ttu-id="9734e-165">Somente os usuários que tiverem sido excluídos permanentemente serão removidos dos grupos.</span><span class="sxs-lookup"><span data-stu-id="9734e-165">Only users that have been permanently deleted are removed from groups.</span></span> <span data-ttu-id="9734e-166">Os usuários que foram excluídos temporariamente mantêm suas participações no grupo e não serão exibidos no resultado delta até que tenham sido excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="9734e-166">Users that have been temporary deleted keep their group memberships and will not appear in the delta result until they are permanently deleted.</span></span> <span data-ttu-id="9734e-167">Para obter mais detalhes, consulte [diretório (itens deletados)](/graph/api/resources/directory?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="9734e-167">For details, see [directory (deleted items)](/graph/api/resources/directory?view=graph-rest-1.0).</span></span>

  - <span data-ttu-id="9734e-168">O segundo usuário foi adicionado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="9734e-168">The second user has been added to the group.</span></span>

## <a name="paging-through-members-in-a-large-group"></a><span data-ttu-id="9734e-169">Ver membros de um grande grupo</span><span class="sxs-lookup"><span data-stu-id="9734e-169">Paging through members in a large group</span></span>

<span data-ttu-id="9734e-170">A propriedade `members@delta` é incluída em objetos de grupo por padrão quando o parâmetro de consulta `$select` não foi especificado ou quando o parâmetro `$select=members` é explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="9734e-170">The `members@delta` property is included in group objects by default, when the `$select` query parameter has not been specified, or when the `$select=members` parameter is explicitly specified.</span></span> <span data-ttu-id="9734e-171">No caso de grupos com muitos membros, é possível que nem todos caibam em uma resposta única. Nesta seção, descrevemos o padrão a ser implementado para lidar com essas situações.</span><span class="sxs-lookup"><span data-stu-id="9734e-171">For groups with many members it is possible that all members cannot fit into a single response; in this section we describe the pattern you should implement to handle such cases.</span></span>

><span data-ttu-id="9734e-172">**Observação:** esse padrão aplica-se à recuperação inicial do estado de grupo e às chamadas subsequentes para obter as alterações da consulta delta.</span><span class="sxs-lookup"><span data-stu-id="9734e-172">**Note:** This pattern applies to both the initial retrieval of group state as well as to subsequent calls to get delta changes.</span></span>

<span data-ttu-id="9734e-173">Vamos supor que você esteja executando a consulta delta a seguir para capturar o estado inicial completo de grupos ou posteriormente para obter alterações da consulta delta:</span><span class="sxs-lookup"><span data-stu-id="9734e-173">Let's assume you are executing the following delta query - either to capture the initial full state of groups, or later on to get delta changes:</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

1. <span data-ttu-id="9734e-174">O Microsoft Graph pode retornar uma resposta com apenas um objeto de grupo, com uma lista grande de membros na propriedade `members@delta`:</span><span class="sxs-lookup"><span data-stu-id="9734e-174">Microsoft Graph may return a response that contains just one group object, with a large list of members in the `members@delta` property:</span></span>

<span data-ttu-id="9734e-175">**Primeira página**</span><span class="sxs-lookup"><span data-stu-id="9734e-175">**First page**</span></span>

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

2. <span data-ttu-id="9734e-176">Quando você seguir o `nextLink`, poderá receber uma resposta novamente com o mesmo objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="9734e-176">When you follow the `nextLink` you may receive a response again containing the same group object.</span></span> <span data-ttu-id="9734e-177">Os mesmos valores de propriedade serão retornados, mas a propriedade `members@delta` agora contém uma lista de usuários diferente.</span><span class="sxs-lookup"><span data-stu-id="9734e-177">The same property values will be returned but the `members@delta` property now contains a different list of users.</span></span>

<span data-ttu-id="9734e-178">**Segunda página**</span><span class="sxs-lookup"><span data-stu-id="9734e-178">**Second page**</span></span>

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

3. <span data-ttu-id="9734e-179">A lista de membros completa será retornada dessa maneira, e outros grupos começarão a aparecer na resposta.</span><span class="sxs-lookup"><span data-stu-id="9734e-179">Eventually, the entire member list will be returned in this fashion, and other groups will start showing up in the response.</span></span>

<span data-ttu-id="9734e-180">As seguintes práticas recomendadas devem ser seguidas para lidar corretamente com esse padrão:</span><span class="sxs-lookup"><span data-stu-id="9734e-180">We recommend the following best practices to correctly handle this pattern:</span></span>
- <span data-ttu-id="9734e-181">Siga sempre o `nextLink` e mescle localmente o estado de cada grupo. Quando receber respostas relacionadas ao mesmo grupo, use-as para criar a lista completa de associação no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9734e-181">Always follow `nextLink` and locally merge each group's state: as you receive responses related to the same group, use them to build the full membership list in your application.</span></span>
- <span data-ttu-id="9734e-182">É aconselhável não presumir uma sequência específica de respostas.</span><span class="sxs-lookup"><span data-stu-id="9734e-182">It is best not to assume a specific sequence of the responses.</span></span> <span data-ttu-id="9734e-183">Suponha que o mesmo grupo possa aparecer em qualquer lugar na sequência do `nextLink` e leve isso em conta na sua lógica de mesclagem.</span><span class="sxs-lookup"><span data-stu-id="9734e-183">Assume that the same group could show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>


## <a name="see-also"></a><span data-ttu-id="9734e-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="9734e-184">See also</span></span>
<span data-ttu-id="9734e-185">Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9734e-185">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
