---
title: 'group: delta'
description: Get recentemente criado, atualizado ou excluído grupos, incluindo as alterações de associação de grupo, sem precisar realizar uma leitura completa da coleção grupo inteiro. Consulte usando Delta consulta para obter detalhes.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 032dc8906c14ad0ea89ca8eda55d4dc53637efe6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936323"
---
# <a name="group-delta"></a><span data-ttu-id="4de95-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="4de95-104">group: delta</span></span>

> <span data-ttu-id="4de95-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4de95-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4de95-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4de95-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4de95-107">Get recentemente criado, atualizado ou excluído grupos, incluindo as alterações de associação de grupo, sem precisar realizar uma leitura completa da coleção grupo inteiro.</span><span class="sxs-lookup"><span data-stu-id="4de95-107">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="4de95-108">Consulte [Usando Delta consulta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="4de95-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="4de95-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="4de95-109">Permissions</span></span>

<span data-ttu-id="4de95-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4de95-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4de95-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4de95-112">Permission type</span></span>      | <span data-ttu-id="4de95-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4de95-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4de95-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4de95-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4de95-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de95-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4de95-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4de95-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de95-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de95-117">Not supported.</span></span>    |
|<span data-ttu-id="4de95-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4de95-118">Application</span></span> | <span data-ttu-id="4de95-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de95-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de95-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4de95-120">HTTP request</span></span>

<span data-ttu-id="4de95-121">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="4de95-121">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="4de95-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="4de95-122">Query parameters</span></span>

<span data-ttu-id="4de95-p105">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-p105">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="4de95-126">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="4de95-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="4de95-127">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="4de95-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="4de95-128">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="4de95-128">Query parameter</span></span> | <span data-ttu-id="4de95-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4de95-129">Type</span></span>  |<span data-ttu-id="4de95-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de95-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4de95-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="4de95-131">$deltatoken</span></span> | <span data-ttu-id="4de95-132">string</span><span class="sxs-lookup"><span data-stu-id="4de95-132">string</span></span> | <span data-ttu-id="4de95-p106">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="4de95-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="4de95-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="4de95-135">$skiptoken</span></span> | <span data-ttu-id="4de95-136">string</span><span class="sxs-lookup"><span data-stu-id="4de95-136">string</span></span> | <span data-ttu-id="4de95-137">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="4de95-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="4de95-138">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="4de95-138">OData query parameters</span></span>

<span data-ttu-id="4de95-139">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-139">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="4de95-p107">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="4de95-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="4de95-142">Você pode usar `$expand=members` para obter as alterações de associação.</span><span class="sxs-lookup"><span data-stu-id="4de95-142">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="4de95-143">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="4de95-143">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="4de95-144">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="4de95-144">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="4de95-145">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="4de95-145">You can filter multiple objects.</span></span> <span data-ttu-id="4de95-146">Por exemplo, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="4de95-146">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="4de95-147">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="4de95-147">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4de95-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4de95-148">Request headers</span></span>

| <span data-ttu-id="4de95-149">Nome</span><span class="sxs-lookup"><span data-stu-id="4de95-149">Name</span></span>       | <span data-ttu-id="4de95-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de95-150">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4de95-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="4de95-151">Authorization</span></span>  | <span data-ttu-id="4de95-152">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="4de95-152">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="4de95-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4de95-153">Content-Type</span></span>  | <span data-ttu-id="4de95-154">application/json</span><span class="sxs-lookup"><span data-stu-id="4de95-154">application/json</span></span> |
| <span data-ttu-id="4de95-155">Preferir</span><span class="sxs-lookup"><span data-stu-id="4de95-155">Prefer</span></span> | <span data-ttu-id="4de95-156">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="4de95-156">return=minimal</span></span> <br><br><span data-ttu-id="4de95-157">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="4de95-157">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="4de95-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4de95-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4de95-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4de95-159">Request body</span></span>

<span data-ttu-id="4de95-160">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4de95-160">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4de95-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de95-161">Response</span></span>

<span data-ttu-id="4de95-162">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-162">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="4de95-163">A resposta também inclui um token de estado que é uma `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="4de95-163">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="4de95-164">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="4de95-164">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="4de95-165">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="4de95-165">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="4de95-166">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-166">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="4de95-167">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="4de95-167">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="4de95-168">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="4de95-168">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="4de95-169">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="4de95-169">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="4de95-170">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="4de95-170">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="4de95-171">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="4de95-171">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="4de95-172">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="4de95-172">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="4de95-173">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="4de95-173">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="4de95-174">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="4de95-174">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="4de95-175">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-175">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="4de95-176">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="4de95-176">This includes properties being set to null value.</span></span>
- <span data-ttu-id="4de95-177">Se a propriedade não tiver sido alterado, o valor antigo está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-177">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="4de95-178">Se a propriedade nunca tiver sido definida antes que ele não será incluído na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="4de95-178">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="4de95-179">**Observação:** Com esse comportamento, examinando a resposta não é possível saber se uma propriedade está mudando ou não.</span><span class="sxs-lookup"><span data-stu-id="4de95-179">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="4de95-180">Além disso, as respostas delta tendem a ser grandes porque eles contêm todos os valores de propriedade - conforme mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="4de95-180">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="4de95-181">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="4de95-181">Alternative: return only the changed properties</span></span>

<span data-ttu-id="4de95-182">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="4de95-182">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="4de95-183">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4de95-183">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="4de95-184">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="4de95-184">This includes properties being set to null value.</span></span>
- <span data-ttu-id="4de95-185">Se a propriedade não tiver sido alterado, a propriedade não está incluída na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="4de95-185">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="4de95-186">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="4de95-186">(Different from the default behavior.)</span></span>

> <span data-ttu-id="4de95-187">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="4de95-187">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="4de95-188">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="4de95-188">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="4de95-189">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="4de95-189">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="4de95-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4de95-190">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="4de95-191">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="4de95-191">Request 1</span></span>

<span data-ttu-id="4de95-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4de95-192">The following is an example of the request.</span></span> <span data-ttu-id="4de95-193">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="4de95-193">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="4de95-194">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="4de95-194">Response 1</span></span>

<span data-ttu-id="4de95-195">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4de95-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="4de95-196">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4de95-196">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4de95-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4de95-197">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="4de95-198">Observe a presença da propriedade *members@delta* que inclui as ids de objetos membros no grupo.</span><span class="sxs-lookup"><span data-stu-id="4de95-198">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
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

#### <a name="request-2"></a><span data-ttu-id="4de95-199">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="4de95-199">Request 2</span></span>

<span data-ttu-id="4de95-200">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="4de95-200">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="4de95-201">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="4de95-201">Response 2</span></span>

<span data-ttu-id="4de95-202">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4de95-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="4de95-203">Observe que todas as 3 propriedades estão incluídas na resposta e não se sabe quais foram alterados desde o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="4de95-203">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="4de95-204">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="4de95-204">Request 3</span></span>

<span data-ttu-id="4de95-205">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="4de95-205">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="4de95-206">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="4de95-206">Response 3</span></span>

<span data-ttu-id="4de95-207">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4de95-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="4de95-208">Observe que o `mailNickname` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `description` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4de95-208">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="4de95-209">Confira também</span><span class="sxs-lookup"><span data-stu-id="4de95-209">See also</span></span>

- <span data-ttu-id="4de95-210">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="4de95-210">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="4de95-211">[Fazer alterações incrementais para grupos](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="4de95-211">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
