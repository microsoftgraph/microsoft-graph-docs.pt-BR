---
title: 'directoryobject: Delta'
description: 'Obter objetos de diretório recém-criados, atualizados ou excluídos dos seguintes tipos: usuário, grupo e contato organizacional, em uma única consulta Delta. Confira Controlar alterações para saber mais.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f3c547d9589c2b94e261113fafca8adc2f70f688
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718223"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="48a73-104">directoryobject: Delta</span><span class="sxs-lookup"><span data-stu-id="48a73-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a73-105">Obter objetos de diretório recém-criados, atualizados ou excluídos dos seguintes tipos: [usuário](../resources/user.md), [grupo](../resources/group.md) e [contato organizacional](../resources/orgcontact.md), em uma única consulta Delta.</span><span class="sxs-lookup"><span data-stu-id="48a73-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="48a73-106">Confira [Controlar alterações](/graph/delta-query-overview) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="48a73-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="48a73-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="48a73-107">Permissions</span></span>

<span data-ttu-id="48a73-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48a73-110">Permission type</span></span>      | <span data-ttu-id="48a73-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48a73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48a73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48a73-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48a73-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48a73-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="48a73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48a73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48a73-115">Not supported.</span></span>  |
|<span data-ttu-id="48a73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48a73-116">Application</span></span> | <span data-ttu-id="48a73-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a73-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48a73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48a73-118">HTTP request</span></span>

<span data-ttu-id="48a73-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso directoryObjects.</span><span class="sxs-lookup"><span data-stu-id="48a73-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="48a73-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="48a73-120">Query parameters</span></span>

<span data-ttu-id="48a73-121">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="48a73-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="48a73-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="48a73-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="48a73-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="48a73-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="48a73-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="48a73-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="48a73-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="48a73-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="48a73-126">Query parameter</span></span> | <span data-ttu-id="48a73-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="48a73-127">Type</span></span> |<span data-ttu-id="48a73-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a73-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48a73-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="48a73-129">$deltatoken</span></span> | <span data-ttu-id="48a73-130">string</span><span class="sxs-lookup"><span data-stu-id="48a73-130">string</span></span> | <span data-ttu-id="48a73-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="48a73-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="48a73-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="48a73-133">$skiptoken</span></span> | <span data-ttu-id="48a73-134">string</span><span class="sxs-lookup"><span data-stu-id="48a73-134">string</span></span> | <span data-ttu-id="48a73-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="48a73-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="48a73-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="48a73-136">OData query parameters</span></span>

<span data-ttu-id="48a73-137">Este método fornece suporte opcional a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="48a73-138">Você pode usar `$filter` com o operador `isOf` especial para filtrar um subconjunto de tipos derivados de directoryobject.</span><span class="sxs-lookup"><span data-stu-id="48a73-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="48a73-139">Você pode combinar várias expressões usando um `or`, que permite que você tenha uma única consulta Delta de acompanhamento de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="48a73-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="48a73-140">Confira o [terceiro exemplo](#request-3) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="48a73-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48a73-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48a73-141">Request headers</span></span>

| <span data-ttu-id="48a73-142">Nome</span><span class="sxs-lookup"><span data-stu-id="48a73-142">Name</span></span>       | <span data-ttu-id="48a73-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a73-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48a73-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="48a73-144">Authorization</span></span>  | <span data-ttu-id="48a73-145">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="48a73-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="48a73-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48a73-146">Content-Type</span></span>  | <span data-ttu-id="48a73-147">application/json</span><span class="sxs-lookup"><span data-stu-id="48a73-147">application/json</span></span> |
| <span data-ttu-id="48a73-148">Preferir</span><span class="sxs-lookup"><span data-stu-id="48a73-148">Prefer</span></span> | <span data-ttu-id="48a73-149">return=minimal</span><span class="sxs-lookup"><span data-stu-id="48a73-149">return=minimal</span></span> <br><br><span data-ttu-id="48a73-150">Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez.</span><span class="sxs-lookup"><span data-stu-id="48a73-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="48a73-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="48a73-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48a73-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48a73-152">Request body</span></span>

<span data-ttu-id="48a73-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48a73-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="48a73-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a73-154">Response</span></span>

<span data-ttu-id="48a73-155">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="48a73-156">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="48a73-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="48a73-157">Se uma URL `nextLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="48a73-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="48a73-158">Existem páginas de dados adicionais a recuperar na sessão.</span><span class="sxs-lookup"><span data-stu-id="48a73-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="48a73-159">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="48a73-160">A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="48a73-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="48a73-161">Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="48a73-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="48a73-162">Se uma URL `deltaLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="48a73-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="48a73-163">Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso.</span><span class="sxs-lookup"><span data-stu-id="48a73-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="48a73-164">Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="48a73-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="48a73-165">Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="48a73-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="48a73-166">Padrão: retornar as mesmas propriedades de uma solicitação delta inicial</span><span class="sxs-lookup"><span data-stu-id="48a73-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="48a73-167">Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="48a73-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="48a73-168">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="48a73-169">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="48a73-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="48a73-170">Se a propriedade não foi alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="48a73-171">Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="48a73-172">**Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="48a73-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="48a73-173">Além disso, as respostas Delta tendem a ser grandes porque contêm todos os valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="48a73-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="48a73-174">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="48a73-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="48a73-175">Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:</span><span class="sxs-lookup"><span data-stu-id="48a73-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="48a73-176">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="48a73-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="48a73-177">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="48a73-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="48a73-178">Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="48a73-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="48a73-179">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="48a73-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="48a73-180">**Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="48a73-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="48a73-181">O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada.</span><span class="sxs-lookup"><span data-stu-id="48a73-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="48a73-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48a73-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="48a73-183">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="48a73-183">Request 1</span></span>

<span data-ttu-id="48a73-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48a73-184">The following is an example of the request.</span></span> <span data-ttu-id="48a73-185">Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="48a73-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48a73-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a73-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48a73-187">C#</span><span class="sxs-lookup"><span data-stu-id="48a73-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48a73-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a73-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48a73-189">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="48a73-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="48a73-190">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="48a73-190">Response 1</span></span>

<span data-ttu-id="48a73-191">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="48a73-191">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="48a73-192">Nenhum `isOf` filtro foi usado, portanto, todos os tipos derivados de directoryobject são retornados.</span><span class="sxs-lookup"><span data-stu-id="48a73-192">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="48a73-193">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48a73-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48a73-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48a73-194">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",      
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="48a73-195">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="48a73-195">Request 2</span></span>

<span data-ttu-id="48a73-196">O exemplo a seguir mostra o uso do comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="48a73-196">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48a73-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a73-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48a73-198">C#</span><span class="sxs-lookup"><span data-stu-id="48a73-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48a73-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a73-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48a73-200">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="48a73-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="48a73-201">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="48a73-201">Response 2</span></span>

<span data-ttu-id="48a73-202">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="48a73-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="48a73-203">Observação apenas as propriedades que realmente foram alteradas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="48a73-203">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="48a73-204">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="48a73-204">Request 3</span></span>

<span data-ttu-id="48a73-205">O próximo exemplo mostra a solicitação inicial usando o `isOf` operador para filtrar somente entidades de usuário e de Grupo:</span><span class="sxs-lookup"><span data-stu-id="48a73-205">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48a73-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a73-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48a73-207">C#</span><span class="sxs-lookup"><span data-stu-id="48a73-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48a73-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a73-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48a73-209">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="48a73-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="48a73-210">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="48a73-210">Response 3</span></span>

<span data-ttu-id="48a73-211">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="48a73-211">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="48a73-212">Observe que somente objetos de usuário e de grupo são retornados:</span><span class="sxs-lookup"><span data-stu-id="48a73-212">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- <span data-ttu-id="48a73-213">[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="48a73-213">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="48a73-214">[Obter as alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="48a73-214">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
