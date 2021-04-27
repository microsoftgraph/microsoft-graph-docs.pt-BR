---
title: 'directoryObject: delta'
description: 'Obter objetos de diretório recém-criados, atualizados ou excluídos dos seguintes tipos: usuário, grupo e contato organizacional, em uma única consulta delta. Confira Controlar alterações para saber mais.'
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 51076a2530b1b1696e271b02e916a74ca0d31516
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046871"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="02055-104">directoryObject: delta</span><span class="sxs-lookup"><span data-stu-id="02055-104">directoryObject: delta</span></span>

<span data-ttu-id="02055-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02055-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02055-106">Obter objetos de diretório recém-criados, atualizados ou [](../resources/group.md) excluídos dos seguintes tipos: [usuário,](../resources/user.md)grupo e contato organizacional [,](../resources/orgcontact.md)em uma única consulta delta.</span><span class="sxs-lookup"><span data-stu-id="02055-106">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="02055-107">Confira [controle de alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="02055-107">See [change tracking](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="02055-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="02055-108">Permissions</span></span>

<span data-ttu-id="02055-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02055-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02055-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02055-111">Permission type</span></span>      | <span data-ttu-id="02055-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02055-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02055-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02055-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02055-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02055-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="02055-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02055-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02055-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02055-116">Not supported.</span></span>  |
|<span data-ttu-id="02055-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02055-117">Application</span></span> | <span data-ttu-id="02055-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02055-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02055-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02055-119">HTTP request</span></span>

<span data-ttu-id="02055-120">Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso directoryObjects.</span><span class="sxs-lookup"><span data-stu-id="02055-120">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="02055-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="02055-121">Query parameters</span></span>

<span data-ttu-id="02055-122">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="02055-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="02055-123">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="02055-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="02055-124">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="02055-125">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="02055-125">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="02055-126">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="02055-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="02055-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="02055-127">Query parameter</span></span> | <span data-ttu-id="02055-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="02055-128">Type</span></span> |<span data-ttu-id="02055-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="02055-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02055-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="02055-130">$deltatoken</span></span> | <span data-ttu-id="02055-131">string</span><span class="sxs-lookup"><span data-stu-id="02055-131">string</span></span> | <span data-ttu-id="02055-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="02055-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="02055-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="02055-134">$skiptoken</span></span> | <span data-ttu-id="02055-135">string</span><span class="sxs-lookup"><span data-stu-id="02055-135">string</span></span> | <span data-ttu-id="02055-136">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="02055-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="02055-137">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="02055-137">OData query parameters</span></span>

<span data-ttu-id="02055-138">Este método fornece suporte opcional a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-138">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="02055-139">Você pode usar `$filter` com o operador especial para `isOf` filtrar um subconjunto de tipos derivados de directoryObject.</span><span class="sxs-lookup"><span data-stu-id="02055-139">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="02055-140">Você pode combinar várias expressões usando um , que permite que você tenha uma `or` única consulta delta monitorando vários tipos.</span><span class="sxs-lookup"><span data-stu-id="02055-140">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="02055-141">Consulte o [terceiro exemplo para](#request-3) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="02055-141">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02055-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02055-142">Request headers</span></span>

| <span data-ttu-id="02055-143">Nome</span><span class="sxs-lookup"><span data-stu-id="02055-143">Name</span></span>       | <span data-ttu-id="02055-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="02055-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02055-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="02055-145">Authorization</span></span>  | <span data-ttu-id="02055-146">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="02055-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="02055-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02055-147">Content-Type</span></span>  | <span data-ttu-id="02055-148">application/json</span><span class="sxs-lookup"><span data-stu-id="02055-148">application/json</span></span> |
| <span data-ttu-id="02055-149">Preferir</span><span class="sxs-lookup"><span data-stu-id="02055-149">Prefer</span></span> | <span data-ttu-id="02055-150">return=minimal</span><span class="sxs-lookup"><span data-stu-id="02055-150">return=minimal</span></span> <br><br><span data-ttu-id="02055-151">Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez.</span><span class="sxs-lookup"><span data-stu-id="02055-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="02055-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02055-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02055-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02055-153">Request body</span></span>

<span data-ttu-id="02055-154">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02055-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="02055-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="02055-155">Response</span></span>

<span data-ttu-id="02055-156">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-156">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="02055-157">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="02055-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="02055-158">Se uma URL `nextLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="02055-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="02055-159">Existem páginas de dados adicionais a recuperar na sessão.</span><span class="sxs-lookup"><span data-stu-id="02055-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="02055-160">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="02055-161">A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="02055-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="02055-162">Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="02055-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="02055-163">Se uma URL `deltaLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="02055-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="02055-164">Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso.</span><span class="sxs-lookup"><span data-stu-id="02055-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="02055-165">Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="02055-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="02055-166">Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="02055-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="02055-167">Padrão: retornar as mesmas propriedades de uma solicitação delta inicial</span><span class="sxs-lookup"><span data-stu-id="02055-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="02055-168">Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="02055-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="02055-169">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-169">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="02055-170">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="02055-170">This includes properties being set to null value.</span></span>
- <span data-ttu-id="02055-171">Se a propriedade não foi alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-171">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="02055-172">Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-172">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="02055-173">**Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="02055-173">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="02055-174">Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="02055-174">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="02055-175">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="02055-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="02055-176">Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:</span><span class="sxs-lookup"><span data-stu-id="02055-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="02055-177">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="02055-177">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="02055-178">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="02055-178">This includes properties being set to null value.</span></span>
- <span data-ttu-id="02055-179">Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="02055-179">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="02055-180">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="02055-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="02055-181">**Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="02055-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="02055-182">O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada.</span><span class="sxs-lookup"><span data-stu-id="02055-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="02055-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02055-183">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="02055-184">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="02055-184">Request 1</span></span>

<span data-ttu-id="02055-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02055-185">The following is an example of the request.</span></span> <span data-ttu-id="02055-186">Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="02055-186">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="02055-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="02055-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="c"></a>[<span data-ttu-id="02055-188">C#</span><span class="sxs-lookup"><span data-stu-id="02055-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02055-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02055-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02055-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02055-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02055-191">Java</span><span class="sxs-lookup"><span data-stu-id="02055-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directory-object-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="02055-192">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="02055-192">Response 1</span></span>

<span data-ttu-id="02055-193">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="02055-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="02055-194">Nenhum filtro foi usado, portanto, todos os `isOf` tipos derivados de directoryObject são retornados.</span><span class="sxs-lookup"><span data-stu-id="02055-194">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="02055-195">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02055-195">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="request-2"></a><span data-ttu-id="02055-196">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="02055-196">Request 2</span></span>

<span data-ttu-id="02055-197">O próximo exemplo mostra o uso do comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="02055-197">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="02055-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="02055-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="02055-199">C#</span><span class="sxs-lookup"><span data-stu-id="02055-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02055-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02055-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02055-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02055-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02055-202">Java</span><span class="sxs-lookup"><span data-stu-id="02055-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="02055-203">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="02055-203">Response 2</span></span>

<span data-ttu-id="02055-204">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="02055-204">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="02055-205">Observe que apenas as propriedades que realmente foram alteradas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="02055-205">Note only the properties that have actually changed are returned.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="02055-206">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="02055-206">Request 3</span></span>

<span data-ttu-id="02055-207">O próximo exemplo mostra a solicitação inicial usando o operador `isOf` para filtrar somente entidades de usuário e grupo:</span><span class="sxs-lookup"><span data-stu-id="02055-207">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="http"></a>[<span data-ttu-id="02055-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="02055-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="c"></a>[<span data-ttu-id="02055-209">C#</span><span class="sxs-lookup"><span data-stu-id="02055-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02055-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02055-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02055-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02055-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02055-212">Java</span><span class="sxs-lookup"><span data-stu-id="02055-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="02055-213">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="02055-213">Response 3</span></span>

<span data-ttu-id="02055-214">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="02055-214">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="02055-215">Observe que somente objetos de usuário e grupo são retornados:</span><span class="sxs-lookup"><span data-stu-id="02055-215">Note that only user and group objects are returned:</span></span>

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

- <span data-ttu-id="02055-216">[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="02055-216">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="02055-217">[Obter as alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="02055-217">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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


