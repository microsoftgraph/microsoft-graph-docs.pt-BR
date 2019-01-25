---
title: 'user: delta'
description: Get recentemente criado, atualizado ou excluído usuários sem precisar realizar uma leitura completa do conjunto de usuários inteira. Consulte controlar alterações para obter detalhes.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508899"
---
# <a name="user-delta"></a><span data-ttu-id="e1c4f-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="e1c4f-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1c4f-105">Get recentemente criado, atualizado ou excluído usuários sem precisar realizar uma leitura completa do conjunto de usuários inteira.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="e1c4f-106">Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1c4f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1c4f-107">Permissions</span></span>

<span data-ttu-id="e1c4f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e1c4f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1c4f-110">Permission type</span></span>      | <span data-ttu-id="e1c4f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1c4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1c4f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1c4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1c4f-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1c4f-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1c4f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1c4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1c4f-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1c4f-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e1c4f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1c4f-116">Application</span></span> | <span data-ttu-id="e1c4f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c4f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1c4f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1c4f-118">HTTP request</span></span>

<span data-ttu-id="e1c4f-119">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="e1c4f-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e1c4f-120">Query parameters</span></span>

<span data-ttu-id="e1c4f-121">Controle de alterações em usuários provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="e1c4f-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="e1c4f-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="e1c4f-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="e1c4f-123">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="e1c4f-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="e1c4f-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e1c4f-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="e1c4f-126">Query parameter</span></span>      | <span data-ttu-id="e1c4f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1c4f-127">Type</span></span>   |<span data-ttu-id="e1c4f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1c4f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1c4f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e1c4f-129">$deltatoken</span></span> | <span data-ttu-id="e1c4f-130">string</span><span class="sxs-lookup"><span data-stu-id="e1c4f-130">string</span></span> | <span data-ttu-id="e1c4f-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e1c4f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e1c4f-133">$skiptoken</span></span> | <span data-ttu-id="e1c4f-134">string</span><span class="sxs-lookup"><span data-stu-id="e1c4f-134">string</span></span> | <span data-ttu-id="e1c4f-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="e1c4f-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="e1c4f-136">OData query parameters</span></span>

<span data-ttu-id="e1c4f-137">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="e1c4f-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="e1c4f-140">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="e1c4f-141">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="e1c4f-142">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-142">You can filter multiple objects.</span></span> <span data-ttu-id="e1c4f-143">Por exemplo, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="e1c4f-144">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1c4f-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1c4f-145">Request headers</span></span>
| <span data-ttu-id="e1c4f-146">Nome</span><span class="sxs-lookup"><span data-stu-id="e1c4f-146">Name</span></span>       | <span data-ttu-id="e1c4f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1c4f-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1c4f-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1c4f-148">Authorization</span></span>  | <span data-ttu-id="e1c4f-149">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="e1c4f-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e1c4f-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1c4f-150">Content-Type</span></span>  | <span data-ttu-id="e1c4f-151">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c4f-151">application/json</span></span> |
| <span data-ttu-id="e1c4f-152">Preferir</span><span class="sxs-lookup"><span data-stu-id="e1c4f-152">Prefer</span></span> | <span data-ttu-id="e1c4f-153">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-153">return=minimal</span></span> <br><br><span data-ttu-id="e1c4f-154">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="e1c4f-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1c4f-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1c4f-156">Request body</span></span>
<span data-ttu-id="e1c4f-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e1c4f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1c4f-158">Response</span></span>

<span data-ttu-id="e1c4f-159">Se tiver êxito, este método retornará `200 OK` objeto de coleção [usuário](../resources/user.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="e1c4f-160">A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="e1c4f-161">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="e1c4f-162">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="e1c4f-163">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="e1c4f-164">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="e1c4f-165">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="e1c4f-166">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="e1c4f-167">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="e1c4f-168">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="e1c4f-169">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="e1c4f-170">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="e1c4f-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="e1c4f-171">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="e1c4f-172">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e1c4f-173">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e1c4f-174">Se a propriedade não tiver sido alterado, o valor antigo está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="e1c4f-175">Se a propriedade nunca tiver sido definida antes que ele não será incluído na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="e1c4f-176">**Observação:** Com esse comportamento, examinando a resposta não é possível saber se uma propriedade está mudando ou não.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="e1c4f-177">Além disso, as respostas delta tendem a ser grandes porque eles contêm todos os valores de propriedade - conforme mostrado no [segundo exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="e1c4f-178">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="e1c4f-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="e1c4f-179">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="e1c4f-180">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e1c4f-181">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e1c4f-182">Se a propriedade não tiver sido alterado, a propriedade não está incluída na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="e1c4f-183">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="e1c4f-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="e1c4f-184">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="e1c4f-185">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="e1c4f-186">Consulte o [terceiro exemplo](#request-3) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="e1c4f-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1c4f-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="e1c4f-188">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e1c4f-188">Request 1</span></span>

<span data-ttu-id="e1c4f-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-189">The following is an example of the request.</span></span> <span data-ttu-id="e1c4f-190">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="e1c4f-191">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e1c4f-191">Response 1</span></span>

<span data-ttu-id="e1c4f-192">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="e1c4f-p119">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="e1c4f-195">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e1c4f-195">Request 2</span></span>

<span data-ttu-id="e1c4f-196">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com o comportamento padrão de resposta:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="e1c4f-197">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e1c4f-197">Response 2</span></span>

<span data-ttu-id="e1c4f-198">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e1c4f-199">Observe que todas as 3 propriedades estão incluídas na resposta e não se sabe quais foram alterados desde o `deltaLink` foi obtido.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="e1c4f-200">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="e1c4f-200">Request 3</span></span>

<span data-ttu-id="e1c4f-201">O exemplo a seguir mostra a solicitação inicial selecionando 3 propriedades de controle de alterações, com comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="e1c4f-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="e1c4f-202">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="e1c4f-202">Response 3</span></span>

<span data-ttu-id="e1c4f-203">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e1c4f-204">Observe que o `mobilePhone` propriedade não for incluída, que significa que ele não tiver sido alterado desde a última consulta delta; `displayName` e `jobTitle` estão incluídos o que significa que seus valores foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e1c4f-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="e1c4f-205">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e1c4f-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="e1c4f-206">Obter as alterações incrementais para usuários</span><span class="sxs-lookup"><span data-stu-id="e1c4f-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
