---
title: 'user: delta'
description: Veja os usuários recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa da coleção de usuários inteira.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95f50b7c839b3936e30e7bdad9b40f0bbfda4136
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820630"
---
# <a name="user-delta"></a><span data-ttu-id="dc50d-103">user: delta</span><span class="sxs-lookup"><span data-stu-id="dc50d-103">user: delta</span></span>

<span data-ttu-id="dc50d-104">Veja os usuários recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa da coleção de usuários inteira.</span><span class="sxs-lookup"><span data-stu-id="dc50d-104">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="dc50d-105">Confira [Controlar alterações](/graph/delta-query-overview) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="dc50d-105">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc50d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc50d-106">Permissions</span></span>

<span data-ttu-id="dc50d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc50d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dc50d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc50d-109">Permission type</span></span>      | <span data-ttu-id="dc50d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc50d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc50d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc50d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc50d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc50d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc50d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc50d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc50d-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc50d-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="dc50d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc50d-115">Application</span></span> | <span data-ttu-id="dc50d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc50d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc50d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc50d-117">HTTP request</span></span>

<span data-ttu-id="dc50d-118">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="dc50d-118">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="dc50d-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="dc50d-119">Query parameters</span></span>

<span data-ttu-id="dc50d-120">O controle de alterações em usuários corresponde a uma série de uma ou mais chamadas de função **delta**.</span><span class="sxs-lookup"><span data-stu-id="dc50d-120">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="dc50d-121">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="dc50d-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="dc50d-122">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="dc50d-123">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="dc50d-123">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="dc50d-124">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="dc50d-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="dc50d-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="dc50d-125">Query parameter</span></span>      | <span data-ttu-id="dc50d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc50d-126">Type</span></span>   |<span data-ttu-id="dc50d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc50d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc50d-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="dc50d-128">$deltatoken</span></span> | <span data-ttu-id="dc50d-129">string</span><span class="sxs-lookup"><span data-stu-id="dc50d-129">string</span></span> | <span data-ttu-id="dc50d-p104">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="dc50d-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="dc50d-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dc50d-132">$skiptoken</span></span> | <span data-ttu-id="dc50d-133">string</span><span class="sxs-lookup"><span data-stu-id="dc50d-133">string</span></span> | <span data-ttu-id="dc50d-134">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="dc50d-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="dc50d-135">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="dc50d-135">OData query parameters</span></span>

<span data-ttu-id="dc50d-136">Este método fornece suporte opcional a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-136">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="dc50d-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="dc50d-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="dc50d-139">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="dc50d-139">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="dc50d-140">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="dc50d-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="dc50d-141">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="dc50d-141">You can filter multiple objects.</span></span> <span data-ttu-id="dc50d-142">Por exemplo, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="dc50d-142">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="dc50d-143">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="dc50d-143">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc50d-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50d-144">Request headers</span></span>
| <span data-ttu-id="dc50d-145">Nome</span><span class="sxs-lookup"><span data-stu-id="dc50d-145">Name</span></span>       | <span data-ttu-id="dc50d-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc50d-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc50d-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc50d-147">Authorization</span></span>  | <span data-ttu-id="dc50d-148">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="dc50d-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="dc50d-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc50d-149">Content-Type</span></span>  | <span data-ttu-id="dc50d-150">application/json</span><span class="sxs-lookup"><span data-stu-id="dc50d-150">application/json</span></span> |
| <span data-ttu-id="dc50d-151">Preferir</span><span class="sxs-lookup"><span data-stu-id="dc50d-151">Prefer</span></span> | <span data-ttu-id="dc50d-152">return=minimal</span><span class="sxs-lookup"><span data-stu-id="dc50d-152">return=minimal</span></span> <br><br><span data-ttu-id="dc50d-153">Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez.</span><span class="sxs-lookup"><span data-stu-id="dc50d-153">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="dc50d-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dc50d-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc50d-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50d-155">Request body</span></span>
<span data-ttu-id="dc50d-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc50d-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc50d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50d-157">Response</span></span>

<span data-ttu-id="dc50d-158">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-158">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="dc50d-159">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="dc50d-159">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="dc50d-160">Se uma URL `nextLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="dc50d-160">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="dc50d-161">Existem páginas de dados adicionais a recuperar na sessão.</span><span class="sxs-lookup"><span data-stu-id="dc50d-161">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="dc50d-162">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-162">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="dc50d-163">A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="dc50d-163">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="dc50d-164">Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-164">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="dc50d-165">Se uma URL `deltaLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="dc50d-165">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="dc50d-166">Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc50d-166">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="dc50d-167">Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="dc50d-167">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="dc50d-168">Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="dc50d-168">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="dc50d-169">Padrão: retornar as mesmas propriedades de uma solicitação delta inicial</span><span class="sxs-lookup"><span data-stu-id="dc50d-169">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="dc50d-170">Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="dc50d-170">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="dc50d-171">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-171">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dc50d-172">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="dc50d-172">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dc50d-173">Se a propriedade não foi alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-173">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="dc50d-174">Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-174">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="dc50d-175">**Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="dc50d-175">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="dc50d-176">Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedades, como mostrado no [Exemplo 2](#example-2-selecting-three-properties).</span><span class="sxs-lookup"><span data-stu-id="dc50d-176">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#example-2-selecting-three-properties) below.</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="dc50d-177">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="dc50d-177">Alternative: return only the changed properties</span></span>

<span data-ttu-id="dc50d-178">Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:</span><span class="sxs-lookup"><span data-stu-id="dc50d-178">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="dc50d-179">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-179">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dc50d-180">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="dc50d-180">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dc50d-181">Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="dc50d-181">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="dc50d-182">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="dc50d-182">(Different from the default behavior.)</span></span>

> <span data-ttu-id="dc50d-183">**Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-183">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="dc50d-184">O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada.</span><span class="sxs-lookup"><span data-stu-id="dc50d-184">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="dc50d-185">Veja o [Exemplo 3](#example-3-alternative-minimal-response-behavior).</span><span class="sxs-lookup"><span data-stu-id="dc50d-185">See Example 3.</span></span>

## <a name="examples"></a><span data-ttu-id="dc50d-186">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc50d-186">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="dc50d-187">Exemplo 1: Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="dc50d-187">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="dc50d-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50d-188">Request</span></span>

<span data-ttu-id="dc50d-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc50d-189">The following is an example of the request.</span></span> <span data-ttu-id="dc50d-190">Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="dc50d-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc50d-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc50d-191">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc50d-192">C#</span><span class="sxs-lookup"><span data-stu-id="dc50d-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc50d-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc50d-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc50d-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc50d-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dc50d-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50d-195">Response</span></span>

<span data-ttu-id="dc50d-196">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="dc50d-p118">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc50d-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="dc50d-199">Exemplo 2: Escolher três propriedades</span><span class="sxs-lookup"><span data-stu-id="dc50d-199">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="dc50d-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50d-200">Request</span></span>

<span data-ttu-id="dc50d-201">O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações com comportamento de resposta padrão.</span><span class="sxs-lookup"><span data-stu-id="dc50d-201">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc50d-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc50d-202">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc50d-203">C#</span><span class="sxs-lookup"><span data-stu-id="dc50d-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc50d-204">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc50d-204">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc50d-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc50d-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dc50d-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50d-206">Response</span></span>

<span data-ttu-id="dc50d-207">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dc50d-208">Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="dc50d-208">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="dc50d-209">Exemplo 3: Comportamento de resposta mínimo alternativo</span><span class="sxs-lookup"><span data-stu-id="dc50d-209">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="dc50d-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50d-210">Request</span></span>

<span data-ttu-id="dc50d-211">O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa.</span><span class="sxs-lookup"><span data-stu-id="dc50d-211">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc50d-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc50d-212">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc50d-213">C#</span><span class="sxs-lookup"><span data-stu-id="dc50d-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc50d-214">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc50d-214">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc50d-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc50d-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dc50d-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50d-216">Response</span></span>

<span data-ttu-id="dc50d-217">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="dc50d-217">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dc50d-218">Observe que a propriedade `mobilePhone` não foi incluída, ou seja, não foi alterada desde a última consulta delta; `displayName` e `jobTitle` foram incluídas, o que significa que os valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dc50d-218">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a><span data-ttu-id="dc50d-219">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc50d-219">See also</span></span>

- <span data-ttu-id="dc50d-220">[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="dc50d-220">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="dc50d-221">[Obter as alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="dc50d-221">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
