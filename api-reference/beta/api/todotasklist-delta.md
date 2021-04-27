---
title: 'todoTaskList: delta'
description: Obter um conjunto de recursos todoTaskList que foram adicionados, excluídos ou removidos em Microsoft To Do.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce5cc7202806b62afcc7f64bcd3b2393f2d31753
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048922"
---
# <a name="todotasklist-delta"></a><span data-ttu-id="d7563-103">todoTaskList: delta</span><span class="sxs-lookup"><span data-stu-id="d7563-103">todoTaskList: delta</span></span>

<span data-ttu-id="d7563-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7563-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7563-105">Obter um conjunto de [recursos todoTaskList](../resources/todotasklist.md) que foram adicionados, excluídos ou removidos em Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="d7563-105">Get a set of [todoTaskList](../resources/todotasklist.md) resources that have been added, deleted, or removed in Microsoft To Do.</span></span>

<span data-ttu-id="d7563-106">Uma **chamada** de função delta para **todoTaskList** é semelhante a uma solicitação GET, exceto que, aplicando adequadamente [tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTaskList**.</span><span class="sxs-lookup"><span data-stu-id="d7563-106">A **delta** function call for **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTaskList**.</span></span> <span data-ttu-id="d7563-107">Isso permite manter e sincronizar um armazenamento local do **todoTaskList** de um usuário sem precisar buscar todas as **todoTaskList** do servidor sempre.</span><span class="sxs-lookup"><span data-stu-id="d7563-107">This allows you to maintain and synchronize a local store of a user's **todoTaskList** without having to fetch all the **todoTaskList** from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7563-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7563-108">Permissions</span></span>
<span data-ttu-id="d7563-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7563-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d7563-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7563-111">Permission type</span></span>      | <span data-ttu-id="d7563-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7563-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7563-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7563-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7563-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7563-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d7563-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7563-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7563-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7563-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d7563-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7563-117">Application</span></span> | <span data-ttu-id="d7563-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d7563-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7563-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7563-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a><span data-ttu-id="d7563-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d7563-120">Query parameters</span></span>

<span data-ttu-id="d7563-121">Controlar alterações nos **recursos todoTaskList** incorre em uma rodada de uma ou mais chamadas de **função delta.**</span><span class="sxs-lookup"><span data-stu-id="d7563-121">Tracking changes in **todoTaskList** resources incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d7563-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="d7563-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d7563-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="d7563-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d7563-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="d7563-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="d7563-125">Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.</span><span class="sxs-lookup"><span data-stu-id="d7563-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d7563-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="d7563-126">Query parameter</span></span>      | <span data-ttu-id="d7563-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7563-127">Type</span></span>   |<span data-ttu-id="d7563-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7563-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7563-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d7563-129">$deltatoken</span></span> | <span data-ttu-id="d7563-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7563-130">string</span></span> | <span data-ttu-id="d7563-131">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção `deltaLink` **todoTaskList,** indicando a conclusão dessa rodada de controle de alterações. </span><span class="sxs-lookup"><span data-stu-id="d7563-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same **todoTaskList** collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d7563-132">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="d7563-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d7563-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d7563-133">$skiptoken</span></span> | <span data-ttu-id="d7563-134">string</span><span class="sxs-lookup"><span data-stu-id="d7563-134">string</span></span> | <span data-ttu-id="d7563-135">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção `nextLink` **todoTaskList.** </span><span class="sxs-lookup"><span data-stu-id="d7563-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same **todoTaskList** collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="d7563-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="d7563-136">OData query parameters</span></span>

<span data-ttu-id="d7563-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="d7563-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="d7563-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7563-139">Request headers</span></span>
| <span data-ttu-id="d7563-140">Nome</span><span class="sxs-lookup"><span data-stu-id="d7563-140">Name</span></span>       | <span data-ttu-id="d7563-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7563-141">Type</span></span> | <span data-ttu-id="d7563-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7563-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="d7563-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7563-143">Authorization</span></span>  | <span data-ttu-id="d7563-144">string</span><span class="sxs-lookup"><span data-stu-id="d7563-144">string</span></span>  | <span data-ttu-id="d7563-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7563-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7563-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7563-147">Content-Type</span></span>  | <span data-ttu-id="d7563-148">string</span><span class="sxs-lookup"><span data-stu-id="d7563-148">string</span></span>  | <span data-ttu-id="d7563-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7563-p107">application/json. Required.</span></span> |
| <span data-ttu-id="d7563-151">Preferir</span><span class="sxs-lookup"><span data-stu-id="d7563-151">Prefer</span></span> | <span data-ttu-id="d7563-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7563-152">string</span></span>  | <span data-ttu-id="d7563-p108">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d7563-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d7563-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7563-155">Response</span></span>

<span data-ttu-id="d7563-156">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7563-156">If successful, this method returns a `200 OK` response code and [todoTaskList](../resources/todotasklist.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7563-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7563-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7563-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7563-158">Request</span></span>
<span data-ttu-id="d7563-159">O exemplo a seguir mostra como fazer uma chamada de função **delta** inicial e limitar o número máximo de **todoTaskList** no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="d7563-159">The following example shows how to make an initial **delta** function call, and limit the maximum number of **todoTaskList** in the response body to 2.</span></span>

<span data-ttu-id="d7563-160">Para controlar as alterações na **todoTaskList,** você faria uma ou mais chamadas de função **delta,** com tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="d7563-160">To track changes in the **todoTaskList**, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="d7563-161">As principais diferenças entre o controle **de todoTaskList** e o controle de recursos **todoTask** em uma lista estão nas URLs de solicitação de consulta delta e as respostas de consulta retornando **todoTaskList** em vez de coleções **todoTask.**</span><span class="sxs-lookup"><span data-stu-id="d7563-161">The main differences between tracking **todoTaskList** and tracking **todoTask** resources in a list are in the delta query request URLs, and the query responses returning **todoTaskList** rather than **todoTask** collections.</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a><span data-ttu-id="d7563-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7563-162">Response</span></span>

<span data-ttu-id="d7563-163">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="d7563-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="d7563-p109">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="d7563-p109">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="d7563-166">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="d7563-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="d7563-167">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7563-167">Note: The response object shown here might be shortened for readability.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d7563-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7563-168">See also</span></span>

- [<span data-ttu-id="d7563-169">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d7563-169">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

