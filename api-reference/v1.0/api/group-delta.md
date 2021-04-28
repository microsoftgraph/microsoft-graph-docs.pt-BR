---
title: 'group: delta'
description: Obter grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação ao grupo, sem precisar executar uma leitura completa de todo o conjunto de grupos.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e094aaae32d8fe4ccbadd534b3d75ece56f8176e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050483"
---
# <a name="group-delta"></a><span data-ttu-id="3200b-103">group: delta</span><span class="sxs-lookup"><span data-stu-id="3200b-103">group: delta</span></span>

<span data-ttu-id="3200b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3200b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3200b-105">Obter grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação ao grupo, sem precisar executar uma leitura completa de todo o conjunto de grupos.</span><span class="sxs-lookup"><span data-stu-id="3200b-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="3200b-106">Consulte [Using Delta Query](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="3200b-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="3200b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3200b-107">Permissions</span></span>

<span data-ttu-id="3200b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3200b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3200b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3200b-110">Permission type</span></span>      | <span data-ttu-id="3200b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3200b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3200b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3200b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3200b-113">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="3200b-113">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="3200b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3200b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3200b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3200b-115">Not supported.</span></span>    |
|<span data-ttu-id="3200b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3200b-116">Application</span></span> | <span data-ttu-id="3200b-117">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3200b-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3200b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3200b-118">HTTP request</span></span>

<span data-ttu-id="3200b-119">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="3200b-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="3200b-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="3200b-120">Query parameters</span></span>

<span data-ttu-id="3200b-p103">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="3200b-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="3200b-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="3200b-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="3200b-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="3200b-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="3200b-126">Query parameter</span></span> | <span data-ttu-id="3200b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3200b-127">Type</span></span>  |<span data-ttu-id="3200b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3200b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3200b-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="3200b-129">$deltatoken</span></span> | <span data-ttu-id="3200b-130">string</span><span class="sxs-lookup"><span data-stu-id="3200b-130">string</span></span> | <span data-ttu-id="3200b-p104">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="3200b-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="3200b-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="3200b-133">$skiptoken</span></span> | <span data-ttu-id="3200b-134">string</span><span class="sxs-lookup"><span data-stu-id="3200b-134">string</span></span> | <span data-ttu-id="3200b-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="3200b-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="3200b-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="3200b-136">OData query parameters</span></span>

<span data-ttu-id="3200b-137">Este método dá suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="3200b-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="3200b-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="3200b-140">Você pode usar `$select=members` para obter alterações de associação.</span><span class="sxs-lookup"><span data-stu-id="3200b-140">You can use `$select=members` to get membership changes.</span></span> <span data-ttu-id="3200b-141">Você também pode rastrear outras alterações, como propriedade e muito mais, selecionando qualquer relação de grupo [do](../resources/group.md#relationships) tipo **coleção directoryObject**.</span><span class="sxs-lookup"><span data-stu-id="3200b-141">You can additionally track other changes like ownership and more by selecting any [group relationship](../resources/group.md#relationships) of type **directoryObject collection**.</span></span>
- <span data-ttu-id="3200b-142">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="3200b-142">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="3200b-143">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="3200b-143">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="3200b-144">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="3200b-144">You can filter multiple objects.</span></span> <span data-ttu-id="3200b-145">Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="3200b-145">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="3200b-146">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="3200b-146">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3200b-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3200b-147">Request headers</span></span>

| <span data-ttu-id="3200b-148">Nome</span><span class="sxs-lookup"><span data-stu-id="3200b-148">Name</span></span>       | <span data-ttu-id="3200b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="3200b-149">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3200b-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="3200b-150">Authorization</span></span>  | <span data-ttu-id="3200b-151">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="3200b-151">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="3200b-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3200b-152">Content-Type</span></span>  | <span data-ttu-id="3200b-153">application/json</span><span class="sxs-lookup"><span data-stu-id="3200b-153">application/json</span></span> |
| <span data-ttu-id="3200b-154">Preferir</span><span class="sxs-lookup"><span data-stu-id="3200b-154">Prefer</span></span> | <span data-ttu-id="3200b-155">return=minimal</span><span class="sxs-lookup"><span data-stu-id="3200b-155">return=minimal</span></span> <br><br><span data-ttu-id="3200b-156">Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez.</span><span class="sxs-lookup"><span data-stu-id="3200b-156">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="3200b-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3200b-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3200b-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3200b-158">Request body</span></span>

<span data-ttu-id="3200b-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3200b-159">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="3200b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3200b-160">Response</span></span>

<span data-ttu-id="3200b-161">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-161">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="3200b-162">A resposta também inclui um token de estado que é uma `nextLink` URL ou uma `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="3200b-162">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="3200b-163">Se uma URL `nextLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="3200b-163">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="3200b-164">Existem páginas de dados adicionais a recuperar na sessão.</span><span class="sxs-lookup"><span data-stu-id="3200b-164">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="3200b-165">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-165">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="3200b-166">A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="3200b-166">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="3200b-167">Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="3200b-167">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="3200b-168">Se uma URL `deltaLink` for retornada:</span><span class="sxs-lookup"><span data-stu-id="3200b-168">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="3200b-169">Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso.</span><span class="sxs-lookup"><span data-stu-id="3200b-169">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="3200b-170">Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="3200b-170">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="3200b-171">Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="3200b-171">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="3200b-172">Padrão: retornar as mesmas propriedades de uma solicitação delta inicial</span><span class="sxs-lookup"><span data-stu-id="3200b-172">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="3200b-173">Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="3200b-173">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="3200b-174">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-174">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="3200b-175">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="3200b-175">This includes properties being set to null value.</span></span>
- <span data-ttu-id="3200b-176">Se a propriedade não foi alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-176">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="3200b-177">Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-177">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="3200b-178">**Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="3200b-178">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="3200b-179">Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedades, como mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="3200b-179">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="3200b-180">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="3200b-180">Alternative: return only the changed properties</span></span>

<span data-ttu-id="3200b-181">Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:</span><span class="sxs-lookup"><span data-stu-id="3200b-181">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="3200b-182">Se a propriedade foi alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="3200b-182">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="3200b-183">Isso inclui propriedades definidas com valor nulo.</span><span class="sxs-lookup"><span data-stu-id="3200b-183">This includes properties being set to null value.</span></span>
- <span data-ttu-id="3200b-184">Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="3200b-184">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="3200b-185">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="3200b-185">(Different from the default behavior.)</span></span>

> <span data-ttu-id="3200b-186">**Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="3200b-186">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="3200b-187">O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada.</span><span class="sxs-lookup"><span data-stu-id="3200b-187">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="3200b-188">Veja o [terceiro exemplo](#request-3) a seguir.</span><span class="sxs-lookup"><span data-stu-id="3200b-188">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="3200b-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3200b-189">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="3200b-190">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="3200b-190">Request 1</span></span>

<span data-ttu-id="3200b-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3200b-191">The following is an example of the request.</span></span> <span data-ttu-id="3200b-192">Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="3200b-192">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="3200b-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="3200b-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta
```
# <a name="c"></a>[<span data-ttu-id="3200b-194">C#</span><span class="sxs-lookup"><span data-stu-id="3200b-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3200b-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3200b-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3200b-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3200b-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3200b-197">Java</span><span class="sxs-lookup"><span data-stu-id="3200b-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a><span data-ttu-id="3200b-198">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="3200b-198">Response 1</span></span>

<span data-ttu-id="3200b-199">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="3200b-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="3200b-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3200b-200">**Note:** The response object shown here might be shortened for readability.</span></span>
>
> <span data-ttu-id="3200b-201">Observe a presença da propriedade *members@delta* que inclui as ids de objetos membros no grupo.</span><span class="sxs-lookup"><span data-stu-id="3200b-201">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
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
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="3200b-202">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="3200b-202">Request 2</span></span>

<span data-ttu-id="3200b-203">O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações, com o comportamento de resposta padrão:</span><span class="sxs-lookup"><span data-stu-id="3200b-203">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="3200b-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="3200b-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```
# <a name="c"></a>[<span data-ttu-id="3200b-205">C#</span><span class="sxs-lookup"><span data-stu-id="3200b-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3200b-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3200b-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3200b-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3200b-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3200b-208">Java</span><span class="sxs-lookup"><span data-stu-id="3200b-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="3200b-209">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="3200b-209">Response 2</span></span>

<span data-ttu-id="3200b-210">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="3200b-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="3200b-211">Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="3200b-211">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="3200b-212">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="3200b-212">Request 3</span></span>

<span data-ttu-id="3200b-213">O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa:</span><span class="sxs-lookup"><span data-stu-id="3200b-213">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="3200b-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="3200b-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="3200b-215">C#</span><span class="sxs-lookup"><span data-stu-id="3200b-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3200b-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3200b-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3200b-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3200b-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3200b-218">Java</span><span class="sxs-lookup"><span data-stu-id="3200b-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a><span data-ttu-id="3200b-219">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="3200b-219">Response 3</span></span>

<span data-ttu-id="3200b-220">A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="3200b-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="3200b-221">Observe que a propriedade `mailNickname` não foi incluída, ou seja, não foi alterada desde a última consulta delta; `displayName` e `description` foram incluídas, o que significa que os valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3200b-221">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="3200b-222">Confira também</span><span class="sxs-lookup"><span data-stu-id="3200b-222">See also</span></span>

- <span data-ttu-id="3200b-223">[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="3200b-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="3200b-224">[Obter alterações incrementais para grupos](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="3200b-224">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

