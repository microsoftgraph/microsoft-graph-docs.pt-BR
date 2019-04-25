---
title: 'user: delta'
description: Obter usuários recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção de usuários. Consulte controlar alterações para obter detalhes.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536998"
---
# <a name="user-delta"></a><span data-ttu-id="bcf20-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="bcf20-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf20-105">Obter usuários recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="bcf20-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="bcf20-106">Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="bcf20-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf20-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcf20-107">Permissions</span></span>

<span data-ttu-id="bcf20-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf20-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bcf20-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcf20-110">Permission type</span></span>      | <span data-ttu-id="bcf20-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcf20-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcf20-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcf20-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcf20-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bcf20-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bcf20-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcf20-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf20-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcf20-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="bcf20-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcf20-116">Application</span></span> | <span data-ttu-id="bcf20-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf20-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcf20-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcf20-118">HTTP request</span></span>

<span data-ttu-id="bcf20-119">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="bcf20-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="bcf20-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="bcf20-120">Query parameters</span></span>

<span data-ttu-id="bcf20-121">O controle de alterações nos usuários provoca uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="bcf20-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="bcf20-122">Se você usar qualquer parâmetro de consulta (diferente `$deltatoken` de `$skiptoken`e), você deve especificá-lo na solicitação de **Delta** inicial.</span><span class="sxs-lookup"><span data-stu-id="bcf20-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="bcf20-123">O Microsoft Graph codifica automaticamente qualquer parâmetro especificado na parte do token do URL `nextLink` ou `deltaLink` na resposta fornecida.</span><span class="sxs-lookup"><span data-stu-id="bcf20-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="bcf20-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="bcf20-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="bcf20-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="bcf20-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="bcf20-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bcf20-126">Query parameter</span></span>      | <span data-ttu-id="bcf20-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcf20-127">Type</span></span>   |<span data-ttu-id="bcf20-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcf20-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcf20-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="bcf20-129">$deltatoken</span></span> | <span data-ttu-id="bcf20-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcf20-130">string</span></span> | <span data-ttu-id="bcf20-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="bcf20-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="bcf20-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="bcf20-133">$skiptoken</span></span> | <span data-ttu-id="bcf20-134">string</span><span class="sxs-lookup"><span data-stu-id="bcf20-134">string</span></span> | <span data-ttu-id="bcf20-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="bcf20-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="bcf20-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="bcf20-136">OData query parameters</span></span>

<span data-ttu-id="bcf20-137">Este método oferece suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="bcf20-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="bcf20-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="bcf20-140">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="bcf20-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="bcf20-141">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="bcf20-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="bcf20-142">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="bcf20-142">You can filter multiple objects.</span></span> <span data-ttu-id="bcf20-143">Por exemplo, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="bcf20-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="bcf20-144">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="bcf20-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf20-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcf20-145">Request headers</span></span>
| <span data-ttu-id="bcf20-146">Nome</span><span class="sxs-lookup"><span data-stu-id="bcf20-146">Name</span></span>       | <span data-ttu-id="bcf20-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcf20-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcf20-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcf20-148">Authorization</span></span>  | <span data-ttu-id="bcf20-149">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="bcf20-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="bcf20-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcf20-150">Content-Type</span></span>  | <span data-ttu-id="bcf20-151">application/json</span><span class="sxs-lookup"><span data-stu-id="bcf20-151">application/json</span></span> |
| <span data-ttu-id="bcf20-152">Preferir</span><span class="sxs-lookup"><span data-stu-id="bcf20-152">Prefer</span></span> | <span data-ttu-id="bcf20-153">retorno = mínimo</span><span class="sxs-lookup"><span data-stu-id="bcf20-153">return=minimal</span></span> <br><br><span data-ttu-id="bcf20-154">A especificação desse cabeçalho com uma solicitação que usa `deltaLink` um retornava apenas as propriedades do objeto que foram alteradas desde a última rodada.</span><span class="sxs-lookup"><span data-stu-id="bcf20-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="bcf20-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bcf20-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf20-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcf20-156">Request body</span></span>
<span data-ttu-id="bcf20-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcf20-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="bcf20-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcf20-158">Response</span></span>

<span data-ttu-id="bcf20-159">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="bcf20-160">A resposta também inclui uma `nextLink` URL ou uma `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="bcf20-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="bcf20-161">Se uma `nextLink` URL for retornada:</span><span class="sxs-lookup"><span data-stu-id="bcf20-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="bcf20-162">Isso indica que há outras páginas de dados a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="bcf20-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="bcf20-163">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="bcf20-164">A resposta inclui o mesmo conjunto de propriedades que na solicitação de consulta Delta inicial.</span><span class="sxs-lookup"><span data-stu-id="bcf20-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="bcf20-165">Isso permite que você capture o estado atual completo dos objetos ao iniciar o ciclo Delta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="bcf20-166">Se uma `deltaLink` URL for retornada:</span><span class="sxs-lookup"><span data-stu-id="bcf20-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="bcf20-167">Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="bcf20-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="bcf20-168">Salve e use a `deltaLink` URL para saber mais sobre as alterações no recurso na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="bcf20-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="bcf20-169">Você tem a opção de especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta somente para as propriedades que foram alteradas desde o momento `deltaLink` em que foi emitido.</span><span class="sxs-lookup"><span data-stu-id="bcf20-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="bcf20-170">Padrão: retornar as mesmas propriedades que a solicitação Delta inicial</span><span class="sxs-lookup"><span data-stu-id="bcf20-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="bcf20-171">Por padrão, as solicitações usando `deltaLink` uma `nextLink` ou retornam as mesmas propriedades selecionadas na consulta Delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="bcf20-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="bcf20-172">Se a propriedade tiver sido alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bcf20-173">Isso inclui propriedades que estão sendo definidas como valor nulo.</span><span class="sxs-lookup"><span data-stu-id="bcf20-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bcf20-174">Se a propriedade não tiver sido alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="bcf20-175">Se a propriedade nunca tiver sido definida antes de não ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="bcf20-176">**Observação:** Com esse comportamento, observando a resposta, não é possível dizer se uma propriedade está sendo alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="bcf20-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="bcf20-177">Além disso, as respostas Delta tendem a ser grandes porque elas contêm todos os valores de propriedade, conforme mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="bcf20-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="bcf20-178">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="bcf20-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="bcf20-179">Adicionar um cabeçalho de solicitação opcional `prefer:return=minimal` --resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="bcf20-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="bcf20-180">Se a propriedade tiver sido alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bcf20-181">Isso inclui propriedades que estão sendo definidas como valor nulo.</span><span class="sxs-lookup"><span data-stu-id="bcf20-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bcf20-182">Se a propriedade não tiver sido alterada, a propriedade não será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="bcf20-183">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="bcf20-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="bcf20-184">**Observação:** O cabeçalho pode ser adicionado a uma `deltaLink` solicitação em um determinado momento no ciclo Delta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="bcf20-185">O cabeçalho afeta apenas o conjunto de propriedades incluído na resposta e não afeta como a consulta Delta é executada.</span><span class="sxs-lookup"><span data-stu-id="bcf20-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="bcf20-186">ConFira o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="bcf20-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="bcf20-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcf20-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="bcf20-188">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="bcf20-188">Request 1</span></span>

<span data-ttu-id="bcf20-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcf20-189">The following is an example of the request.</span></span> <span data-ttu-id="bcf20-190">Não há nenhum `$select` parâmetro, portanto, um conjunto padrão de propriedades é rastreado e retornado.</span><span class="sxs-lookup"><span data-stu-id="bcf20-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="bcf20-191">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="bcf20-191">Response 1</span></span>

<span data-ttu-id="bcf20-192">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="bcf20-193">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcf20-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bcf20-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcf20-194">All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="bcf20-195">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="bcf20-195">Request 2</span></span>

<span data-ttu-id="bcf20-196">O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para o controle de alterações, com comportamento de resposta padrão:</span><span class="sxs-lookup"><span data-stu-id="bcf20-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="bcf20-197">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="bcf20-197">Response 2</span></span>

<span data-ttu-id="bcf20-198">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bcf20-199">Observe que todas as 3 propriedades estão incluídas na resposta e não são conhecidas quais foram alteradas desde que `deltaLink` foram obtidas.</span><span class="sxs-lookup"><span data-stu-id="bcf20-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="bcf20-200">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="bcf20-200">Request 3</span></span>

<span data-ttu-id="bcf20-201">O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="bcf20-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="bcf20-202">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="bcf20-202">Response 3</span></span>

<span data-ttu-id="bcf20-203">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="bcf20-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bcf20-204">Observe que a `mobilePhone` propriedade não é incluída, o que significa que ela não foi alterada desde a última consulta Delta; `displayName` e `jobTitle` são incluídos, o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bcf20-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="bcf20-205">[Usar a consulta Delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="bcf20-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="bcf20-206">[Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="bcf20-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
