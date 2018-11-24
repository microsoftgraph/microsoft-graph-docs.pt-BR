# <a name="user-delta"></a><span data-ttu-id="b7079-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="b7079-101">user: delta</span></span>

<span data-ttu-id="b7079-102">Get recentemente criado, atualizado ou excluído usuários sem precisar realizar uma leitura completa do conjunto de usuários inteira.</span><span class="sxs-lookup"><span data-stu-id="b7079-102">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="b7079-103">Consulte [controlar alterações](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="b7079-103">See [Track changes](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7079-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="b7079-104">Permissions</span></span>

<span data-ttu-id="b7079-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b7079-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b7079-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7079-107">Permission type</span></span>      | <span data-ttu-id="b7079-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7079-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7079-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7079-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b7079-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7079-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7079-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7079-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7079-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7079-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="b7079-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7079-113">Application</span></span> | <span data-ttu-id="b7079-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7079-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7079-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7079-115">HTTP request</span></span>

<span data-ttu-id="b7079-116">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="b7079-116">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b7079-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b7079-117">Query parameters</span></span>

<span data-ttu-id="b7079-118">Controle de alterações em usuários provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="b7079-118">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b7079-119">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="b7079-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b7079-120">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="b7079-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b7079-121">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="b7079-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="b7079-122">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="b7079-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="b7079-123">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="b7079-123">Query parameter</span></span>      | <span data-ttu-id="b7079-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7079-124">Type</span></span>   |<span data-ttu-id="b7079-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7079-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b7079-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b7079-126">$deltatoken</span></span> | <span data-ttu-id="b7079-127">string</span><span class="sxs-lookup"><span data-stu-id="b7079-127">string</span></span> | <span data-ttu-id="b7079-p104">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="b7079-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b7079-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b7079-130">$skiptoken</span></span> | <span data-ttu-id="b7079-131">string</span><span class="sxs-lookup"><span data-stu-id="b7079-131">string</span></span> | <span data-ttu-id="b7079-132">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="b7079-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="b7079-133">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="b7079-133">OData query parameters</span></span>

<span data-ttu-id="b7079-134">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7079-134">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="b7079-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="b7079-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="b7079-137">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="b7079-137">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="b7079-138">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="b7079-138">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="b7079-139">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="b7079-139">You can filter multiple objects.</span></span> <span data-ttu-id="b7079-140">Por exemplo, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="b7079-140">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="b7079-141">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="b7079-141">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7079-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7079-142">Request headers</span></span>
| <span data-ttu-id="b7079-143">Nome</span><span class="sxs-lookup"><span data-stu-id="b7079-143">Name</span></span>       | <span data-ttu-id="b7079-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7079-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7079-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7079-145">Authorization</span></span>  | <span data-ttu-id="b7079-146">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="b7079-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="b7079-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7079-147">Content-Type</span></span>  | <span data-ttu-id="b7079-148">application/json</span><span class="sxs-lookup"><span data-stu-id="b7079-148">application/json</span></span> |
| <span data-ttu-id="b7079-149">Preferir</span><span class="sxs-lookup"><span data-stu-id="b7079-149">Prefer</span></span> | <span data-ttu-id="b7079-150">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="b7079-150">return=minimal</span></span> <br><br><span data-ttu-id="b7079-151">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="b7079-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="b7079-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b7079-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7079-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7079-153">Request body</span></span>
<span data-ttu-id="b7079-154">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7079-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="b7079-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7079-155">Response</span></span>

<span data-ttu-id="b7079-156">Se tiver êxito, este método retornará `200 OK` objeto de coleção [usuário](../resources/user.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7079-156">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="b7079-157">A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="b7079-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="b7079-158">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="b7079-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="b7079-159">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="b7079-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b7079-160">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="b7079-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="b7079-161">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="b7079-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="b7079-162">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="b7079-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="b7079-163">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="b7079-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="b7079-164">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b7079-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b7079-165">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="b7079-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="b7079-166">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="b7079-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="b7079-167">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="b7079-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="b7079-168">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="b7079-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="b7079-169">Se a propriedade foi alterada, retorne a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="b7079-169">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="b7079-170">Se a propriedade tiver sido definida para um valor vazio, retorna o valor da propriedade como null.</span><span class="sxs-lookup"><span data-stu-id="b7079-170">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="b7079-171">Se a propriedade não tiver sido alterado, retorne o valor como null.</span><span class="sxs-lookup"><span data-stu-id="b7079-171">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="b7079-172">**Observação:** Com o comportamento acima, não é possível diferenciar entre uma propriedade que não tiver sido alterado e o que foi alterado para um `null` valor.</span><span class="sxs-lookup"><span data-stu-id="b7079-172">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="b7079-173">Consulte o [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="b7079-173">See the [second example](#request-2) below.</span></span> <span data-ttu-id="b7079-174">Se isso é importante, é recomendável usar o comportamento alternativo descrito na próxima seção.</span><span class="sxs-lookup"><span data-stu-id="b7079-174">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="b7079-175">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="b7079-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="b7079-176">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="b7079-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="b7079-177">Se a propriedade foi alterada, retorne a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="b7079-177">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="b7079-178">Se a propriedade tiver sido definida para um valor vazio, retorna o valor da propriedade como null.</span><span class="sxs-lookup"><span data-stu-id="b7079-178">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="b7079-179">Se a propriedade não tiver sido alterado, não inclua a propriedade na resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="b7079-179">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="b7079-180">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="b7079-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="b7079-181">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="b7079-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="b7079-182">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="b7079-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="b7079-183">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="b7079-183">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="b7079-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7079-184">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="b7079-185">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b7079-185">Request 1</span></span>

<span data-ttu-id="b7079-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7079-186">The following is an example of the request.</span></span> <span data-ttu-id="b7079-187">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="b7079-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="b7079-188">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b7079-188">Response 1</span></span>

<span data-ttu-id="b7079-189">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="b7079-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="b7079-p116">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7079-p116">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="b7079-192">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b7079-192">Request 2</span></span>

<span data-ttu-id="b7079-193">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="b7079-193">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="b7079-194">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b7079-194">Response 2</span></span>

<span data-ttu-id="b7079-195">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="b7079-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b7079-196">Observe que `jobTitle` e `mobilePhone` têm o valor do `null` que significa que eles talvez não tenham sido alterados ou tem sido definidos como um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="b7079-196">Note that `jobTitle` and `mobilePhone` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

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
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="b7079-197">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="b7079-197">Request 3</span></span>

<span data-ttu-id="b7079-198">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="b7079-198">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="b7079-199">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="b7079-199">Response 3</span></span>

<span data-ttu-id="b7079-200">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="b7079-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b7079-201">Observe que o `mobilePhone` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `jobTitle` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b7079-201">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="b7079-202">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="b7079-202">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="b7079-203">[Fazer alterações incrementais para usuários](../../../concepts/delta_query_users.md).</span><span class="sxs-lookup"><span data-stu-id="b7079-203">[Get incremental changes for users](../../../concepts/delta_query_users.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->