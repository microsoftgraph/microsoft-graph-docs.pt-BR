# <a name="group-delta"></a><span data-ttu-id="7da91-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="7da91-101">group: delta</span></span>
<span data-ttu-id="7da91-102">Get recentemente criado, atualizado ou excluído grupos, incluindo as alterações de associação de grupo, sem precisar realizar uma leitura completa da coleção grupo inteiro.</span><span class="sxs-lookup"><span data-stu-id="7da91-102">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="7da91-103">Consulte [Usando Delta consulta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="7da91-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="7da91-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="7da91-104">Permissions</span></span>

<span data-ttu-id="7da91-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7da91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7da91-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7da91-107">Permission type</span></span>      | <span data-ttu-id="7da91-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7da91-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7da91-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7da91-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7da91-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da91-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7da91-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7da91-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7da91-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7da91-112">Not supported.</span></span>    |
|<span data-ttu-id="7da91-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7da91-113">Application</span></span> | <span data-ttu-id="7da91-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da91-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7da91-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7da91-115">HTTP request</span></span>

<span data-ttu-id="7da91-116">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="7da91-116">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="7da91-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="7da91-117">Query parameters</span></span>

<span data-ttu-id="7da91-p103">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="7da91-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="7da91-121">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="7da91-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="7da91-122">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="7da91-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7da91-123">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="7da91-123">Query parameter</span></span> | <span data-ttu-id="7da91-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7da91-124">Type</span></span>  |<span data-ttu-id="7da91-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da91-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7da91-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7da91-126">$deltatoken</span></span> | <span data-ttu-id="7da91-127">string</span><span class="sxs-lookup"><span data-stu-id="7da91-127">string</span></span> | <span data-ttu-id="7da91-p104">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="7da91-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7da91-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7da91-130">$skiptoken</span></span> | <span data-ttu-id="7da91-131">string</span><span class="sxs-lookup"><span data-stu-id="7da91-131">string</span></span> | <span data-ttu-id="7da91-132">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="7da91-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="7da91-133">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="7da91-133">OData query parameters</span></span>

<span data-ttu-id="7da91-134">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7da91-134">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="7da91-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="7da91-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="7da91-137">Você pode usar `$expand=members` para obter as alterações de associação.</span><span class="sxs-lookup"><span data-stu-id="7da91-137">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="7da91-138">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="7da91-138">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="7da91-139">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="7da91-139">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="7da91-140">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="7da91-140">You can filter multiple objects.</span></span> <span data-ttu-id="7da91-141">Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="7da91-141">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="7da91-142">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="7da91-142">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7da91-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7da91-143">Request headers</span></span>

| <span data-ttu-id="7da91-144">Nome</span><span class="sxs-lookup"><span data-stu-id="7da91-144">Name</span></span>       | <span data-ttu-id="7da91-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da91-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7da91-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="7da91-146">Authorization</span></span>  | <span data-ttu-id="7da91-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="7da91-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="7da91-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7da91-148">Content-Type</span></span>  | <span data-ttu-id="7da91-149">application/json</span><span class="sxs-lookup"><span data-stu-id="7da91-149">application/json</span></span> |
| <span data-ttu-id="7da91-150">Preferir</span><span class="sxs-lookup"><span data-stu-id="7da91-150">Prefer</span></span> | <span data-ttu-id="7da91-151">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="7da91-151">return=minimal</span></span> <br><br><span data-ttu-id="7da91-152">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="7da91-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="7da91-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7da91-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7da91-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7da91-154">Request body</span></span>

<span data-ttu-id="7da91-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7da91-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7da91-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da91-156">Response</span></span>

<span data-ttu-id="7da91-157">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7da91-157">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="7da91-158">A resposta também inclui um token de estado que é uma `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="7da91-158">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="7da91-159">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="7da91-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="7da91-160">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="7da91-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7da91-161">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="7da91-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="7da91-162">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="7da91-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="7da91-163">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="7da91-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="7da91-164">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="7da91-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="7da91-165">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="7da91-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7da91-166">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="7da91-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="7da91-167">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="7da91-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="7da91-168">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="7da91-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="7da91-169">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="7da91-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="7da91-170">Se a propriedade foi alterada, retorne a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="7da91-170">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="7da91-171">Se a propriedade tiver sido definida para um valor vazio, retorna o valor da propriedade como null.</span><span class="sxs-lookup"><span data-stu-id="7da91-171">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="7da91-172">Se a propriedade não tiver sido alterado, retorne o valor como null.</span><span class="sxs-lookup"><span data-stu-id="7da91-172">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="7da91-173">**Observação:** Com o comportamento acima, não é possível diferenciar entre uma propriedade que não tiver sido alterado e o que foi alterado para um `null` valor.</span><span class="sxs-lookup"><span data-stu-id="7da91-173">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="7da91-174">Consulte o [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="7da91-174">See the [second example](#request-2) below.</span></span> <span data-ttu-id="7da91-175">Se isso é importante, é recomendável usar o comportamento alternativo descrito na próxima seção.</span><span class="sxs-lookup"><span data-stu-id="7da91-175">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="7da91-176">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="7da91-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="7da91-177">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="7da91-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="7da91-178">Se a propriedade foi alterada, retorne a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="7da91-178">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="7da91-179">Se a propriedade tiver sido definida para um valor vazio, retorna o valor da propriedade como null.</span><span class="sxs-lookup"><span data-stu-id="7da91-179">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="7da91-180">Se a propriedade não tiver sido alterado, não inclua a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="7da91-180">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="7da91-181">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="7da91-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="7da91-182">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="7da91-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="7da91-183">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="7da91-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="7da91-184">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="7da91-184">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="7da91-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7da91-185">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="7da91-186">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="7da91-186">Request 1</span></span>

<span data-ttu-id="7da91-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7da91-187">The following is an example of the request.</span></span> <span data-ttu-id="7da91-188">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="7da91-188">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="7da91-189">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="7da91-189">Response 1</span></span>

<span data-ttu-id="7da91-190">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="7da91-190">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="7da91-191">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7da91-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7da91-192">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7da91-192">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="7da91-193">Observe a presença da propriedade *members@delta* que inclui as ids de objetos membros no grupo.</span><span class="sxs-lookup"><span data-stu-id="7da91-193">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="7da91-194">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="7da91-194">Request 2</span></span>

<span data-ttu-id="7da91-195">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="7da91-195">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="7da91-196">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="7da91-196">Response 2</span></span>

<span data-ttu-id="7da91-197">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="7da91-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="7da91-198">Observe que `description` e `mailNickname` têm o valor do `null` que significa que eles talvez não tenham sido alterados ou tem sido definidos como um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="7da91-198">Note that `description` and `mailNickname` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

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
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="7da91-199">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="7da91-199">Request 3</span></span>

<span data-ttu-id="7da91-200">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="7da91-200">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="7da91-201">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="7da91-201">Response 3</span></span>

<span data-ttu-id="7da91-202">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="7da91-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="7da91-203">Observe que o `mailNickname` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `description` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7da91-203">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7da91-204">Confira também</span><span class="sxs-lookup"><span data-stu-id="7da91-204">See also</span></span>

- <span data-ttu-id="7da91-205">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="7da91-205">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="7da91-206">[Fazer alterações incrementais para grupos](../../../concepts/delta_query_groups.md).</span><span class="sxs-lookup"><span data-stu-id="7da91-206">[Get incremental changes for groups](../../../concepts/delta_query_groups.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
