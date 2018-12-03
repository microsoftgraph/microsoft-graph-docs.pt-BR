---
title: 'group: delta'
description: Get recentemente criado, atualizado ou excluído grupos, incluindo as alterações de associação de grupo, sem precisar realizar uma leitura completa da coleção grupo inteiro. Consulte usando Delta consulta para obter detalhes.
ms.openlocfilehash: c893f72fbd85e69db75121b0d9ef6c69a582afda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007361"
---
# <a name="group-delta"></a><span data-ttu-id="6ba1c-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="6ba1c-104">group: delta</span></span>
<span data-ttu-id="6ba1c-105">Get recentemente criado, atualizado ou excluído grupos, incluindo as alterações de associação de grupo, sem precisar realizar uma leitura completa da coleção grupo inteiro.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="6ba1c-106">Consulte [Usando Delta consulta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ba1c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6ba1c-107">Permissions</span></span>

<span data-ttu-id="6ba1c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ba1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ba1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ba1c-110">Permission type</span></span>      | <span data-ttu-id="6ba1c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ba1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ba1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ba1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ba1c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba1c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ba1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ba1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ba1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-115">Not supported.</span></span>    |
|<span data-ttu-id="6ba1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ba1c-116">Application</span></span> | <span data-ttu-id="6ba1c-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba1c-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ba1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ba1c-118">HTTP request</span></span>

<span data-ttu-id="6ba1c-119">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="6ba1c-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="6ba1c-120">Query parameters</span></span>

<span data-ttu-id="6ba1c-p104">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="6ba1c-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="6ba1c-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="6ba1c-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="6ba1c-126">Query parameter</span></span> | <span data-ttu-id="6ba1c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ba1c-127">Type</span></span>  |<span data-ttu-id="6ba1c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ba1c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ba1c-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="6ba1c-129">$deltatoken</span></span> | <span data-ttu-id="6ba1c-130">string</span><span class="sxs-lookup"><span data-stu-id="6ba1c-130">string</span></span> | <span data-ttu-id="6ba1c-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="6ba1c-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="6ba1c-133">$skiptoken</span></span> | <span data-ttu-id="6ba1c-134">string</span><span class="sxs-lookup"><span data-stu-id="6ba1c-134">string</span></span> | <span data-ttu-id="6ba1c-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="6ba1c-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="6ba1c-136">OData query parameters</span></span>

<span data-ttu-id="6ba1c-137">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="6ba1c-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="6ba1c-140">Você pode usar `$expand=members` para obter as alterações de associação.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="6ba1c-141">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="6ba1c-142">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="6ba1c-143">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-143">You can filter multiple objects.</span></span> <span data-ttu-id="6ba1c-144">Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-144">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="6ba1c-145">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ba1c-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba1c-146">Request headers</span></span>

| <span data-ttu-id="6ba1c-147">Nome</span><span class="sxs-lookup"><span data-stu-id="6ba1c-147">Name</span></span>       | <span data-ttu-id="6ba1c-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ba1c-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ba1c-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ba1c-149">Authorization</span></span>  | <span data-ttu-id="6ba1c-150">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="6ba1c-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="6ba1c-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ba1c-151">Content-Type</span></span>  | <span data-ttu-id="6ba1c-152">application/json</span><span class="sxs-lookup"><span data-stu-id="6ba1c-152">application/json</span></span> |
| <span data-ttu-id="6ba1c-153">Preferir</span><span class="sxs-lookup"><span data-stu-id="6ba1c-153">Prefer</span></span> | <span data-ttu-id="6ba1c-154">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="6ba1c-154">return=minimal</span></span> <br><br><span data-ttu-id="6ba1c-155">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="6ba1c-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ba1c-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba1c-157">Request body</span></span>

<span data-ttu-id="6ba1c-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6ba1c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ba1c-159">Response</span></span>

<span data-ttu-id="6ba1c-160">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="6ba1c-161">A resposta também inclui um token de estado que é uma `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="6ba1c-162">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="6ba1c-163">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="6ba1c-164">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="6ba1c-165">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="6ba1c-166">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="6ba1c-167">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="6ba1c-168">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="6ba1c-169">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="6ba1c-170">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="6ba1c-171">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="6ba1c-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="6ba1c-172">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="6ba1c-173">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6ba1c-174">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6ba1c-175">Se a propriedade não tiver sido alterado, o valor antigo está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="6ba1c-176">Se a propriedade nunca tiver sido definida antes que ele não será incluído na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="6ba1c-177">**Observação:** Com esse comportamento, examinando a resposta não é possível saber se uma propriedade está mudando ou não.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="6ba1c-178">Além disso, as respostas delta tendem a ser grandes porque eles contêm todos os valores de propriedade - conforme mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="6ba1c-179">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="6ba1c-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="6ba1c-180">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="6ba1c-181">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6ba1c-182">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6ba1c-183">Se a propriedade não tiver sido alterado, a propriedade não está incluída na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="6ba1c-184">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="6ba1c-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="6ba1c-185">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="6ba1c-186">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="6ba1c-187">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="6ba1c-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ba1c-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="6ba1c-189">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="6ba1c-189">Request 1</span></span>

<span data-ttu-id="6ba1c-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-190">The following is an example of the request.</span></span> <span data-ttu-id="6ba1c-191">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="6ba1c-192">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="6ba1c-192">Response 1</span></span>

<span data-ttu-id="6ba1c-193">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="6ba1c-194">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6ba1c-195">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-195">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="6ba1c-196">Observe a presença da propriedade *members@delta* que inclui as ids de objetos membros no grupo.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-196">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="6ba1c-197">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="6ba1c-197">Request 2</span></span>

<span data-ttu-id="6ba1c-198">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="6ba1c-199">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="6ba1c-199">Response 2</span></span>

<span data-ttu-id="6ba1c-200">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6ba1c-201">Observe que todas as 3 propriedades estão incluídas na resposta e não se sabe quais foram alterados desde o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="6ba1c-202">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="6ba1c-202">Request 3</span></span>

<span data-ttu-id="6ba1c-203">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="6ba1c-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="6ba1c-204">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="6ba1c-204">Response 3</span></span>

<span data-ttu-id="6ba1c-205">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6ba1c-206">Observe que o `mailNickname` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `description` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6ba1c-206">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6ba1c-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ba1c-207">See also</span></span>

- <span data-ttu-id="6ba1c-208">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="6ba1c-208">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="6ba1c-209">[Fazer alterações incrementais para grupos](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="6ba1c-209">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
