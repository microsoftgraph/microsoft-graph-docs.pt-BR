---
title: 'todoTaskList: Delta'
description: Obtenha um conjunto de recursos do todoTaskList que foram adicionados, excluídos ou removidos no Microsoft para o.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9719b4c9379a79172cc4052439dc4e8abb72b716
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796581"
---
# <a name="todotasklist-delta"></a><span data-ttu-id="69f40-103">todoTaskList: Delta</span><span class="sxs-lookup"><span data-stu-id="69f40-103">todoTaskList: delta</span></span>

<span data-ttu-id="69f40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f40-105">Obtenha um conjunto de recursos do [todoTaskList](../resources/todotasklist.md) que foram adicionados, excluídos ou removidos no Microsoft para o.</span><span class="sxs-lookup"><span data-stu-id="69f40-105">Get a set of [todoTaskList](../resources/todotasklist.md) resources that have been added, deleted, or removed in Microsoft To Do.</span></span>

<span data-ttu-id="69f40-106">Uma chamada de função **Delta** para **todoTaskList** é semelhante a uma solicitação GET, exceto pelo fato de que, por meio da aplicação adequada de [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTaskList** .</span><span class="sxs-lookup"><span data-stu-id="69f40-106">A **delta** function call for **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTaskList** .</span></span> <span data-ttu-id="69f40-107">Isso permite que você mantenha e sincronize um repositório local do **todoTaskList** de um usuário sem ter que buscar todo o **todoTaskList** do servidor a cada vez.</span><span class="sxs-lookup"><span data-stu-id="69f40-107">This allows you to maintain and synchronize a local store of a user's **todoTaskList** without having to fetch all the **todoTaskList** from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f40-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="69f40-108">Permissions</span></span>
<span data-ttu-id="69f40-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69f40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69f40-111">Permission type</span></span>      | <span data-ttu-id="69f40-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69f40-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f40-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69f40-113">Delegated (work or school account)</span></span> | <span data-ttu-id="69f40-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69f40-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69f40-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69f40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f40-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69f40-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69f40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69f40-117">Application</span></span> | <span data-ttu-id="69f40-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="69f40-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69f40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a><span data-ttu-id="69f40-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="69f40-120">Query parameters</span></span>

<span data-ttu-id="69f40-121">O controle de alterações nos recursos do **todoTaskList** provoca uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="69f40-121">Tracking changes in **todoTaskList** resources incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="69f40-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta** .</span><span class="sxs-lookup"><span data-stu-id="69f40-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="69f40-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="69f40-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="69f40-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="69f40-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="69f40-125">Em solicitações subsequentes, basta copiar e aplicar `nextLink` a `deltaLink` URL ou da resposta anterior, pois essa URL já inclui os parâmetros codificados e desejados.</span><span class="sxs-lookup"><span data-stu-id="69f40-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="69f40-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="69f40-126">Query parameter</span></span>      | <span data-ttu-id="69f40-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="69f40-127">Type</span></span>   |<span data-ttu-id="69f40-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f40-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69f40-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="69f40-129">$deltatoken</span></span> | <span data-ttu-id="69f40-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69f40-130">string</span></span> | <span data-ttu-id="69f40-131">Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção **todoTaskList** , indicando a conclusão dessa rodada de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="69f40-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same **todoTaskList** collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="69f40-132">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="69f40-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="69f40-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="69f40-133">$skiptoken</span></span> | <span data-ttu-id="69f40-134">string</span><span class="sxs-lookup"><span data-stu-id="69f40-134">string</span></span> | <span data-ttu-id="69f40-135">Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção **todoTaskList** .</span><span class="sxs-lookup"><span data-stu-id="69f40-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same **todoTaskList** collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="69f40-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="69f40-136">OData query parameters</span></span>

<span data-ttu-id="69f40-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="69f40-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="69f40-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69f40-139">Request headers</span></span>
| <span data-ttu-id="69f40-140">Nome</span><span class="sxs-lookup"><span data-stu-id="69f40-140">Name</span></span>       | <span data-ttu-id="69f40-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="69f40-141">Type</span></span> | <span data-ttu-id="69f40-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f40-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="69f40-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="69f40-143">Authorization</span></span>  | <span data-ttu-id="69f40-144">string</span><span class="sxs-lookup"><span data-stu-id="69f40-144">string</span></span>  | <span data-ttu-id="69f40-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69f40-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69f40-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69f40-147">Content-Type</span></span>  | <span data-ttu-id="69f40-148">string</span><span class="sxs-lookup"><span data-stu-id="69f40-148">string</span></span>  | <span data-ttu-id="69f40-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69f40-p107">application/json. Required.</span></span> |
| <span data-ttu-id="69f40-151">Preferir</span><span class="sxs-lookup"><span data-stu-id="69f40-151">Prefer</span></span> | <span data-ttu-id="69f40-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69f40-152">string</span></span>  | <span data-ttu-id="69f40-p108">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="69f40-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="69f40-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f40-155">Response</span></span>

<span data-ttu-id="69f40-156">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto da coleção [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69f40-156">If successful, this method returns a `200 OK` response code and [todoTaskList](../resources/todotasklist.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f40-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69f40-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="69f40-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69f40-158">Request</span></span>
<span data-ttu-id="69f40-159">O exemplo a seguir mostra como fazer uma chamada de função **Delta** inicial e limitar o número máximo de **todoTaskList** no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="69f40-159">The following example shows how to make an initial **delta** function call, and limit the maximum number of **todoTaskList** in the response body to 2.</span></span>

<span data-ttu-id="69f40-160">Para controlar as alterações no **todoTaskList** , faça uma ou mais chamadas de função **Delta** , com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta Delta.</span><span class="sxs-lookup"><span data-stu-id="69f40-160">To track changes in the **todoTaskList** , you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="69f40-161">As principais diferenças entre o acompanhamento de **todoTaskList** e o acompanhamento de recursos do **todoTask** em uma lista estão nas URLs de solicitação de consulta Delta e as respostas de consulta retornando **TodoTaskList** em vez de conjuntos **todoTask** .</span><span class="sxs-lookup"><span data-stu-id="69f40-161">The main differences between tracking **todoTaskList** and tracking **todoTask** resources in a list are in the delta query request URLs, and the query responses returning **todoTaskList** rather than **todoTask** collections.</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a><span data-ttu-id="69f40-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f40-162">Response</span></span>

<span data-ttu-id="69f40-163">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="69f40-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="69f40-p109">(em um cabeçalho de resposta _@odata.nextLink_ ) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_ ). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="69f40-p109">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="69f40-166">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_ .</span><span class="sxs-lookup"><span data-stu-id="69f40-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="69f40-p110">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69f40-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="69f40-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="69f40-169">See also</span></span>

- [<span data-ttu-id="69f40-170">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="69f40-170">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

