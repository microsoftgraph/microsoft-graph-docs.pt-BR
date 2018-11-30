---
title: 'user: delta'
description: Get recentemente criado, atualizado ou excluído usuários sem precisar realizar uma leitura completa do conjunto de usuários inteira. Consulte controlar alterações para obter detalhes.
ms.openlocfilehash: 7c87f3e0da6e79f2f8a316a214c1408cf2fa7ebc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040806"
---
# <a name="user-delta"></a><span data-ttu-id="4f099-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="4f099-104">user: delta</span></span>

> <span data-ttu-id="4f099-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f099-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f099-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f099-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f099-107">Get recentemente criado, atualizado ou excluído usuários sem precisar realizar uma leitura completa do conjunto de usuários inteira.</span><span class="sxs-lookup"><span data-stu-id="4f099-107">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="4f099-108">Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="4f099-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f099-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f099-109">Permissions</span></span>

<span data-ttu-id="4f099-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f099-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4f099-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f099-112">Permission type</span></span>      | <span data-ttu-id="4f099-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f099-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f099-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f099-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f099-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f099-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f099-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f099-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f099-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f099-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="4f099-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f099-118">Application</span></span> | <span data-ttu-id="4f099-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f099-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f099-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f099-120">HTTP request</span></span>

<span data-ttu-id="4f099-121">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="4f099-121">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="4f099-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="4f099-122">Query parameters</span></span>

<span data-ttu-id="4f099-123">Controle de alterações em usuários provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="4f099-123">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="4f099-124">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="4f099-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="4f099-125">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="4f099-126">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="4f099-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="4f099-127">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="4f099-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="4f099-128">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="4f099-128">Query parameter</span></span>      | <span data-ttu-id="4f099-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f099-129">Type</span></span>   |<span data-ttu-id="4f099-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f099-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f099-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="4f099-131">$deltatoken</span></span> | <span data-ttu-id="4f099-132">string</span><span class="sxs-lookup"><span data-stu-id="4f099-132">string</span></span> | <span data-ttu-id="4f099-p106">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="4f099-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="4f099-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="4f099-135">$skiptoken</span></span> | <span data-ttu-id="4f099-136">string</span><span class="sxs-lookup"><span data-stu-id="4f099-136">string</span></span> | <span data-ttu-id="4f099-137">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="4f099-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="4f099-138">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="4f099-138">OData query parameters</span></span>

<span data-ttu-id="4f099-139">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="4f099-p107">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="4f099-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="4f099-142">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="4f099-142">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="4f099-143">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="4f099-143">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="4f099-144">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="4f099-144">You can filter multiple objects.</span></span> <span data-ttu-id="4f099-145">Por exemplo, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="4f099-145">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="4f099-146">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="4f099-146">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f099-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f099-147">Request headers</span></span>
| <span data-ttu-id="4f099-148">Nome</span><span class="sxs-lookup"><span data-stu-id="4f099-148">Name</span></span>       | <span data-ttu-id="4f099-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f099-149">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f099-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f099-150">Authorization</span></span>  | <span data-ttu-id="4f099-151">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="4f099-151">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="4f099-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f099-152">Content-Type</span></span>  | <span data-ttu-id="4f099-153">application/json</span><span class="sxs-lookup"><span data-stu-id="4f099-153">application/json</span></span> |
| <span data-ttu-id="4f099-154">Preferir</span><span class="sxs-lookup"><span data-stu-id="4f099-154">Prefer</span></span> | <span data-ttu-id="4f099-155">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="4f099-155">return=minimal</span></span> <br><br><span data-ttu-id="4f099-156">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="4f099-156">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="4f099-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4f099-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f099-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f099-158">Request body</span></span>
<span data-ttu-id="4f099-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f099-159">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4f099-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f099-160">Response</span></span>

<span data-ttu-id="4f099-161">Se tiver êxito, este método retornará `200 OK` objeto de coleção [usuário](../resources/user.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-161">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="4f099-162">A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="4f099-162">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="4f099-163">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="4f099-163">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="4f099-164">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="4f099-164">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="4f099-165">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-165">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="4f099-166">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="4f099-166">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="4f099-167">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="4f099-167">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="4f099-168">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="4f099-168">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="4f099-169">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="4f099-169">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="4f099-170">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="4f099-170">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="4f099-171">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="4f099-171">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="4f099-172">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="4f099-172">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="4f099-173">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="4f099-173">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="4f099-174">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-174">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="4f099-175">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="4f099-175">This includes properties being set to null value.</span></span>
- <span data-ttu-id="4f099-176">Se a propriedade não tiver sido alterado, o valor antigo está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-176">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="4f099-177">Se a propriedade nunca tiver sido definida antes que ele não será incluído na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="4f099-177">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="4f099-178">**Observação:** Com esse comportamento, examinando a resposta não é possível saber se uma propriedade está mudando ou não.</span><span class="sxs-lookup"><span data-stu-id="4f099-178">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="4f099-179">Além disso, as respostas delta tendem a ser grandes porque eles contêm todos os valores de propriedade - conforme mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="4f099-179">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="4f099-180">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="4f099-180">Alternative: return only the changed properties</span></span>

<span data-ttu-id="4f099-181">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="4f099-181">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="4f099-182">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="4f099-182">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="4f099-183">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="4f099-183">This includes properties being set to null value.</span></span>
- <span data-ttu-id="4f099-184">Se a propriedade não tiver sido alterado, a propriedade não está incluída na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="4f099-184">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="4f099-185">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="4f099-185">(Different from the default behavior.)</span></span>

> <span data-ttu-id="4f099-186">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="4f099-186">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="4f099-187">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="4f099-187">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="4f099-188">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="4f099-188">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="4f099-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f099-189">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="4f099-190">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="4f099-190">Request 1</span></span>

<span data-ttu-id="4f099-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f099-191">The following is an example of the request.</span></span> <span data-ttu-id="4f099-192">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="4f099-192">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="4f099-193">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="4f099-193">Response 1</span></span>

<span data-ttu-id="4f099-194">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4f099-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="4f099-p120">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f099-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

#### <a name="request-2"></a><span data-ttu-id="4f099-197">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="4f099-197">Request 2</span></span>

<span data-ttu-id="4f099-198">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="4f099-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="4f099-199">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="4f099-199">Response 2</span></span>

<span data-ttu-id="4f099-200">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4f099-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="4f099-201">Observe que todas as 3 propriedades estão incluídas na resposta e não se sabe quais foram alterados desde o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="4f099-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="4f099-202">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="4f099-202">Request 3</span></span>

<span data-ttu-id="4f099-203">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="4f099-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="4f099-204">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="4f099-204">Response 3</span></span>

<span data-ttu-id="4f099-205">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="4f099-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="4f099-206">Observe que o `mobilePhone` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `jobTitle` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4f099-206">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="4f099-207">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="4f099-207">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="4f099-208">[Fazer alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="4f099-208">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
