---
title: 'orgContact: delta'
description: Obter contatos organizacionais recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: afdf3ba022ec5138849fb3cee0732a50d44aef8e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055572"
---
# <a name="orgcontact-delta"></a><span data-ttu-id="758c0-103">orgContact: delta</span><span class="sxs-lookup"><span data-stu-id="758c0-103">orgContact: delta</span></span>

<span data-ttu-id="758c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="758c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758c0-105">Obter contatos organizacionais recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="758c0-105">Get newly created, updated, or deleted organizational contacts without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="758c0-106">Confira [controle de alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="758c0-106">See [change tracking](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="758c0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="758c0-107">Permissions</span></span>

<span data-ttu-id="758c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="758c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="758c0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="758c0-110">Permission type</span></span>      | <span data-ttu-id="758c0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="758c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="758c0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="758c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="758c0-113">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="758c0-113">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="758c0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="758c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="758c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="758c0-115">Not supported.</span></span>  |
|<span data-ttu-id="758c0-116">Application</span><span class="sxs-lookup"><span data-stu-id="758c0-116">Application</span></span> | <span data-ttu-id="758c0-117">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="758c0-117">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="758c0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="758c0-118">HTTP request</span></span>

<span data-ttu-id="758c0-119">Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso contatos.</span><span class="sxs-lookup"><span data-stu-id="758c0-119">To begin tracking changes, you make a request including the delta function on the contacts resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="758c0-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="758c0-120">Query parameters</span></span>

<span data-ttu-id="758c0-121">O controle de alterações em contatos organizacionais incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="758c0-121">Tracking changes in organizational contacts incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="758c0-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="758c0-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="758c0-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="758c0-124">Você só precisa especificar os parâmetros de consulta uma vez na frente.</span><span class="sxs-lookup"><span data-stu-id="758c0-124">You only need to specify any query parameters once up front.</span></span>

<span data-ttu-id="758c0-125">Em solicitações subsequentes, copie e aplique `nextLink` a URL ou da resposta `deltaLink` anterior.</span><span class="sxs-lookup"><span data-stu-id="758c0-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="758c0-126">Essa URL já inclui os parâmetros codificados.</span><span class="sxs-lookup"><span data-stu-id="758c0-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="758c0-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="758c0-127">Query parameter</span></span>      | <span data-ttu-id="758c0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="758c0-128">Type</span></span>   |<span data-ttu-id="758c0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="758c0-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="758c0-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="758c0-130">$deltatoken</span></span> | <span data-ttu-id="758c0-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="758c0-131">string</span></span> | <span data-ttu-id="758c0-132">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de contatos da organização, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="758c0-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same organization contact collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="758c0-133">Salve e aplique a URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle `deltaLink` de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="758c0-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="758c0-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="758c0-134">$skiptoken</span></span> | <span data-ttu-id="758c0-135">string</span><span class="sxs-lookup"><span data-stu-id="758c0-135">string</span></span> | <span data-ttu-id="758c0-136">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção `nextLink` de contatos da organização. </span><span class="sxs-lookup"><span data-stu-id="758c0-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same organization contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="758c0-137">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="758c0-137">OData query parameters</span></span>

<span data-ttu-id="758c0-138">Este método dá suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-138">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="758c0-139">Você pode usar um parâmetro de consulta como em qualquer solicitação GET para especificar apenas as `$select` propriedades de que você precisa para obter o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="758c0-139">You can use a `$select` query parameter as in any GET request to specify only the properties you need for best performance.</span></span> <span data-ttu-id="758c0-140">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="758c0-140">The **id** property is always returned.</span></span>
- <span data-ttu-id="758c0-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="758c0-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="758c0-142">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="758c0-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="758c0-143">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="758c0-143">You can filter multiple objects.</span></span> <span data-ttu-id="758c0-144">Por exemplo, `https://graph.microsoft.com/beta/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="758c0-144">For example, `https://graph.microsoft.com/beta/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="758c0-145">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="758c0-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="758c0-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="758c0-146">Request headers</span></span>
| <span data-ttu-id="758c0-147">Nome</span><span class="sxs-lookup"><span data-stu-id="758c0-147">Name</span></span>       | <span data-ttu-id="758c0-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="758c0-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="758c0-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="758c0-149">Authorization</span></span>  | <span data-ttu-id="758c0-p108">&lt;token&gt; de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="758c0-p108">Bearer &lt;token&gt;. Required.</span></span>|
| <span data-ttu-id="758c0-152">Preferir</span><span class="sxs-lookup"><span data-stu-id="758c0-152">Prefer</span></span> | <span data-ttu-id="758c0-153">return=minimal</span><span class="sxs-lookup"><span data-stu-id="758c0-153">return=minimal</span></span> <br><br><span data-ttu-id="758c0-154">Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez.</span><span class="sxs-lookup"><span data-stu-id="758c0-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="758c0-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="758c0-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="758c0-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="758c0-156">Request body</span></span>
<span data-ttu-id="758c0-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="758c0-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="758c0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="758c0-158">Response</span></span>

<span data-ttu-id="758c0-159">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-159">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) collection object in the response body.</span></span> <span data-ttu-id="758c0-160">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="758c0-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="758c0-161">Se uma URL `nextLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="758c0-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="758c0-162">Existem páginas de dados adicionais a recuperar na sessão.</span><span class="sxs-lookup"><span data-stu-id="758c0-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="758c0-163">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="758c0-164">A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="758c0-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="758c0-165">Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="758c0-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="758c0-166">Se uma URL `deltaLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="758c0-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="758c0-167">Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="758c0-167">This indicates that there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="758c0-168">Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="758c0-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="758c0-169">Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="758c0-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="758c0-170">Padrão: retornar as mesmas propriedades de uma solicitação delta inicial</span><span class="sxs-lookup"><span data-stu-id="758c0-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="758c0-171">Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="758c0-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="758c0-172">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="758c0-173">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="758c0-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="758c0-174">Se a propriedade não foi alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="758c0-175">Se a propriedade nunca tiver sido definida antes, ela não será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-175">If the property has never been set before, it will not be included in the response at all.</span></span>


> <span data-ttu-id="758c0-176">**Observação:** Com esse comportamento, não é possível dizer se uma propriedade está mudando olhando para a resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-176">**Note:** With this behavior, it is not possible to tell whether a property is changing by looking at the response.</span></span> <span data-ttu-id="758c0-177">Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedade - conforme mostrado no [Exemplo 2](#example-2-selecting-three-properties).</span><span class="sxs-lookup"><span data-stu-id="758c0-177">Also, the delta responses tend to be large because they contain all property values - as shown in [Example 2](#example-2-selecting-three-properties).</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="758c0-178">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="758c0-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="758c0-179">Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:</span><span class="sxs-lookup"><span data-stu-id="758c0-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="758c0-180">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="758c0-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="758c0-181">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="758c0-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="758c0-182">Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="758c0-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="758c0-183">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="758c0-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="758c0-184">**Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="758c0-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="758c0-185">O header afeta apenas o conjunto de propriedades incluídas na resposta e não afeta como a consulta delta é executado.</span><span class="sxs-lookup"><span data-stu-id="758c0-185">The header only affects the set of properties included in the response and it does not affect how the delta query is run.</span></span> <span data-ttu-id="758c0-186">Veja o [Exemplo 3](#example-3-alternative-minimal-response-behavior).</span><span class="sxs-lookup"><span data-stu-id="758c0-186">See [Example 3](#example-3-alternative-minimal-response-behavior).</span></span>

## <a name="examples"></a><span data-ttu-id="758c0-187">Exemplos</span><span class="sxs-lookup"><span data-stu-id="758c0-187">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="758c0-188">Exemplo 1: Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="758c0-188">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="758c0-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="758c0-189">Request</span></span>

<span data-ttu-id="758c0-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="758c0-190">The following is an example of the request.</span></span> <span data-ttu-id="758c0-191">Como não há `$select` parâmetro, um conjunto padrão de propriedades é rastreado e retornado.</span><span class="sxs-lookup"><span data-stu-id="758c0-191">Because there is no `$select` parameter, a default set of properties is tracked and returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="758c0-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="758c0-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta
```
# <a name="c"></a>[<span data-ttu-id="758c0-193">C#</span><span class="sxs-lookup"><span data-stu-id="758c0-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="758c0-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="758c0-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="758c0-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="758c0-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="758c0-196">Java</span><span class="sxs-lookup"><span data-stu-id="758c0-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="758c0-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="758c0-197">Response</span></span>

<span data-ttu-id="758c0-198">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="758c0-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="758c0-199">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="758c0-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="758c0-200">Exemplo 2: Escolher três propriedades</span><span class="sxs-lookup"><span data-stu-id="758c0-200">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="758c0-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="758c0-201">Request</span></span>

<span data-ttu-id="758c0-202">O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações com comportamento de resposta padrão.</span><span class="sxs-lookup"><span data-stu-id="758c0-202">The next example shows the initial request selecting three properties for change tracking, with default response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="758c0-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="758c0-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
```
# <a name="c"></a>[<span data-ttu-id="758c0-204">C#</span><span class="sxs-lookup"><span data-stu-id="758c0-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="758c0-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="758c0-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="758c0-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="758c0-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="758c0-207">Java</span><span class="sxs-lookup"><span data-stu-id="758c0-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="758c0-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="758c0-208">Response</span></span>

<span data-ttu-id="758c0-209">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="758c0-209">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="758c0-210">Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="758c0-210">Note that all three properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="758c0-211">Exemplo 3: Comportamento de resposta mínimo alternativo</span><span class="sxs-lookup"><span data-stu-id="758c0-211">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="758c0-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="758c0-212">Request</span></span>

<span data-ttu-id="758c0-213">O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa.</span><span class="sxs-lookup"><span data-stu-id="758c0-213">The next example shows the initial request selecting three properties for change tracking, with alternative minimal response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="758c0-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="758c0-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="758c0-215">C#</span><span class="sxs-lookup"><span data-stu-id="758c0-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="758c0-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="758c0-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="758c0-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="758c0-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="758c0-218">Java</span><span class="sxs-lookup"><span data-stu-id="758c0-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="758c0-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="758c0-219">Response</span></span>

<span data-ttu-id="758c0-220">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="758c0-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="758c0-221">Observe que a propriedade não está incluída, o que significa que ela não foi alterada desde a última consulta delta; e estão incluídas, o que significa que seus `mail` `displayName` valores foram `jobTitle` alterados.</span><span class="sxs-lookup"><span data-stu-id="758c0-221">Note that the `mail` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included, which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a><span data-ttu-id="758c0-222">Confira também</span><span class="sxs-lookup"><span data-stu-id="758c0-222">See also</span></span>

- <span data-ttu-id="758c0-223">[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="758c0-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


