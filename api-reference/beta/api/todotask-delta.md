---
title: 'todoTask: delta'
description: Obter um conjunto de recursos todoTask que foram adicionados, excluídos ou atualizados em um todoTaskList especificado.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3c0d1759d1994c1fa9ae405d2a1895982e3ac99a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048915"
---
# <a name="todotask-delta"></a><span data-ttu-id="40488-103">todoTask: delta</span><span class="sxs-lookup"><span data-stu-id="40488-103">todoTask: delta</span></span>

<span data-ttu-id="40488-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40488-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40488-105">Obter um conjunto de [recursos todoTask](../resources/todotask.md) que foram adicionados, excluídos ou atualizados em [um todoTaskList especificado.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="40488-105">Get a set of [todoTask](../resources/todotask.md) resources that have been added, deleted, or updated in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

<span data-ttu-id="40488-106">Uma **chamada** de função delta para recursos **todoTask** em **um todoTaskList** é semelhante a uma solicitação GET, exceto que, aplicando [adequadamente tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTask** em **todoTaskList**.</span><span class="sxs-lookup"><span data-stu-id="40488-106">A **delta** function call for **todoTask** resources in a **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTask** in that **todoTaskList**.</span></span> <span data-ttu-id="40488-107">Isso permite manter e sincronizar um armazenamento local dos recursos **todoTask** de um usuário sem precisar buscar todo o conjunto do servidor sempre.</span><span class="sxs-lookup"><span data-stu-id="40488-107">This allows you to maintain and synchronize a local store of a user's **todoTask** resources without having to fetch the entire set from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="40488-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="40488-108">Permissions</span></span>
<span data-ttu-id="40488-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40488-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40488-111">Permission type</span></span>      | <span data-ttu-id="40488-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40488-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40488-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40488-113">Delegated (work or school account)</span></span> | <span data-ttu-id="40488-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40488-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="40488-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40488-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40488-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40488-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="40488-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40488-117">Application</span></span> | <span data-ttu-id="40488-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="40488-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="40488-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40488-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a><span data-ttu-id="40488-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="40488-120">Query parameters</span></span>

<span data-ttu-id="40488-121">Controlar alterações em uma **coleção todoTask** incorre em uma rodada de uma ou mais chamadas de **função delta.**</span><span class="sxs-lookup"><span data-stu-id="40488-121">Tracking changes in a **todoTask** collection incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="40488-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="40488-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="40488-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="40488-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="40488-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="40488-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="40488-125">Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.</span><span class="sxs-lookup"><span data-stu-id="40488-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="40488-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="40488-126">Query parameter</span></span>      | <span data-ttu-id="40488-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="40488-127">Type</span></span>   |<span data-ttu-id="40488-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="40488-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40488-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="40488-129">$deltatoken</span></span> | <span data-ttu-id="40488-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40488-130">string</span></span> | <span data-ttu-id="40488-131">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção `deltaLink` todoTask, indicando a conclusão dessa rodada de controle de alterações. </span><span class="sxs-lookup"><span data-stu-id="40488-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same todoTask collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="40488-132">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="40488-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="40488-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="40488-133">$skiptoken</span></span> | <span data-ttu-id="40488-134">string</span><span class="sxs-lookup"><span data-stu-id="40488-134">string</span></span> | <span data-ttu-id="40488-135">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção `nextLink` todoTask. </span><span class="sxs-lookup"><span data-stu-id="40488-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same todoTask collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="40488-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="40488-136">OData query parameters</span></span>

- <span data-ttu-id="40488-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="40488-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="40488-139">Suporte à consulta `$select` delta , e para `$top` `$expand` todoTask.</span><span class="sxs-lookup"><span data-stu-id="40488-139">Delta query support `$select`, `$top`, and `$expand` for todoTask.</span></span> 
- <span data-ttu-id="40488-140">Há suporte limitado para `$filter` e `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="40488-140">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="40488-141">As únicas expressões `$filter` com suporte são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="40488-141">The only supported `$filter` expressions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="40488-p106">A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.</span><span class="sxs-lookup"><span data-stu-id="40488-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="40488-144">Não há suporte para `$search`.</span><span class="sxs-lookup"><span data-stu-id="40488-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40488-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40488-145">Request headers</span></span>
| <span data-ttu-id="40488-146">Nome</span><span class="sxs-lookup"><span data-stu-id="40488-146">Name</span></span>       | <span data-ttu-id="40488-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="40488-147">Type</span></span> | <span data-ttu-id="40488-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="40488-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="40488-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="40488-149">Authorization</span></span>  | <span data-ttu-id="40488-150">string</span><span class="sxs-lookup"><span data-stu-id="40488-150">string</span></span>  | <span data-ttu-id="40488-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40488-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40488-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40488-153">Content-Type</span></span>  | <span data-ttu-id="40488-154">string</span><span class="sxs-lookup"><span data-stu-id="40488-154">string</span></span>  | <span data-ttu-id="40488-p108">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40488-p108">application/json. Required.</span></span> |
| <span data-ttu-id="40488-157">Preferir</span><span class="sxs-lookup"><span data-stu-id="40488-157">Prefer</span></span> | <span data-ttu-id="40488-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40488-158">string</span></span>  | <span data-ttu-id="40488-p109">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="40488-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="40488-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="40488-161">Response</span></span>

<span data-ttu-id="40488-162">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40488-162">If successful, this method returns a `200 OK` response code and [todoTask](../resources/todotask.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40488-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40488-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="40488-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40488-164">Request</span></span>
<span data-ttu-id="40488-165">Para controlar as alterações nos recursos **todoTask** em um **todoTaskList** desde a última rodada de controle de alterações, você faria uma ou mais chamadas de função **delta** para obter o conjunto de alterações incrementais.</span><span class="sxs-lookup"><span data-stu-id="40488-165">To track changes in the **todoTask** resources in a **todoTaskList** since the last round of change tracking, you would make one or more **delta** function calls to get the set of incremental changes.</span></span> <span data-ttu-id="40488-166">O exemplo a seguir mostra como iniciar uma próxima rodada de controle de alterações, usando a URL na chamada de última função delta da última rodada, que contém `deltaLink` um  `deltaToken` .</span><span class="sxs-lookup"><span data-stu-id="40488-166">The following example shows how to begin a next round of change tracking, using the URL in the `deltaLink` returned from the last **delta** function call of the last round, which contains a `deltaToken`.</span></span> <span data-ttu-id="40488-167">Essa **chamada** de função delta limita o número máximo de **todoTask** no corpo da resposta como 2.</span><span class="sxs-lookup"><span data-stu-id="40488-167">This **delta** function call limits the maximum number of **todoTask** in the response body to 2.</span></span>
 

### <a name="http-request"></a><span data-ttu-id="40488-168">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40488-168">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
Prefer: odata.maxpagesize=2
```


### <a name="response"></a><span data-ttu-id="40488-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="40488-169">Response</span></span>
<span data-ttu-id="40488-170">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="40488-170">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="40488-p111">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="40488-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="40488-173">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="40488-173">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="40488-174">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40488-174">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
   "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
   "value":[
      {
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      }
   ]
}
```

## <a name="see-also"></a><span data-ttu-id="40488-175">Confira também</span><span class="sxs-lookup"><span data-stu-id="40488-175">See also</span></span>

- [<span data-ttu-id="40488-176">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="40488-176">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

