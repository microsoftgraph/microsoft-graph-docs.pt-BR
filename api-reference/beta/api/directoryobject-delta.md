---
title: 'directoryobject: Delta'
description: 'Obter objetos de diretório recém-criados, atualizados ou excluídos dos seguintes tipos: usuário, grupo e contato organizacional, em uma única consulta Delta. Consulte controlar alterações para obter detalhes.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9dd3c835070581314b1620c0012237c9beca5b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326056"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="b6916-104">directoryobject: Delta</span><span class="sxs-lookup"><span data-stu-id="b6916-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6916-105">Obter objetos de diretório recém-criados, atualizados ou excluídos dos seguintes tipos: [usuário](../resources/user.md), [grupo](../resources/group.md) e [contato organizacional](../resources/orgcontact.md), em uma única consulta Delta.</span><span class="sxs-lookup"><span data-stu-id="b6916-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="b6916-106">Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="b6916-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6916-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6916-107">Permissions</span></span>

<span data-ttu-id="b6916-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6916-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6916-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6916-110">Permission type</span></span>      | <span data-ttu-id="b6916-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6916-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6916-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6916-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6916-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6916-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="b6916-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6916-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6916-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6916-115">Not supported.</span></span>  |
|<span data-ttu-id="b6916-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6916-116">Application</span></span> | <span data-ttu-id="b6916-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6916-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6916-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6916-118">HTTP request</span></span>

<span data-ttu-id="b6916-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso directoryObjects.</span><span class="sxs-lookup"><span data-stu-id="b6916-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b6916-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b6916-120">Query parameters</span></span>

<span data-ttu-id="b6916-121">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="b6916-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b6916-122">Se você usar qualquer parâmetro de consulta (diferente `$deltatoken` de `$skiptoken`e), você deve especificá-lo na solicitação de **Delta** inicial.</span><span class="sxs-lookup"><span data-stu-id="b6916-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b6916-123">O Microsoft Graph codifica automaticamente qualquer parâmetro especificado na parte do token do URL `nextLink` ou `deltaLink` na resposta fornecida.</span><span class="sxs-lookup"><span data-stu-id="b6916-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b6916-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="b6916-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="b6916-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="b6916-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="b6916-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="b6916-126">Query parameter</span></span> | <span data-ttu-id="b6916-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6916-127">Type</span></span> |<span data-ttu-id="b6916-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6916-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6916-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b6916-129">$deltatoken</span></span> | <span data-ttu-id="b6916-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6916-130">string</span></span> | <span data-ttu-id="b6916-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="b6916-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b6916-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b6916-133">$skiptoken</span></span> | <span data-ttu-id="b6916-134">string</span><span class="sxs-lookup"><span data-stu-id="b6916-134">string</span></span> | <span data-ttu-id="b6916-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="b6916-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="b6916-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="b6916-136">OData query parameters</span></span>

<span data-ttu-id="b6916-137">Este método oferece suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="b6916-138">Você pode usar `$filter` com o operador `isOf` especial para filtrar um subconjunto de tipos derivados de directoryobject.</span><span class="sxs-lookup"><span data-stu-id="b6916-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="b6916-139">Você pode combinar várias expressões usando um `or`, que permite que você tenha uma única consulta Delta de acompanhamento de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="b6916-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="b6916-140">ConFira o [terceiro exemplo](#request-3) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="b6916-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6916-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6916-141">Request headers</span></span>

| <span data-ttu-id="b6916-142">Nome</span><span class="sxs-lookup"><span data-stu-id="b6916-142">Name</span></span>       | <span data-ttu-id="b6916-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6916-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6916-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6916-144">Authorization</span></span>  | <span data-ttu-id="b6916-145">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="b6916-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="b6916-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6916-146">Content-Type</span></span>  | <span data-ttu-id="b6916-147">application/json</span><span class="sxs-lookup"><span data-stu-id="b6916-147">application/json</span></span> |
| <span data-ttu-id="b6916-148">Preferir</span><span class="sxs-lookup"><span data-stu-id="b6916-148">Prefer</span></span> | <span data-ttu-id="b6916-149">retorno = mínimo</span><span class="sxs-lookup"><span data-stu-id="b6916-149">return=minimal</span></span> <br><br><span data-ttu-id="b6916-150">A especificação desse cabeçalho com uma solicitação que usa `deltaLink` um retornava apenas as propriedades do objeto que foram alteradas desde a última rodada.</span><span class="sxs-lookup"><span data-stu-id="b6916-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="b6916-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6916-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6916-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6916-152">Request body</span></span>

<span data-ttu-id="b6916-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6916-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="b6916-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6916-154">Response</span></span>

<span data-ttu-id="b6916-155">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="b6916-156">A resposta também inclui uma `nextLink` URL ou uma `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="b6916-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="b6916-157">Se uma `nextLink` URL for retornada:</span><span class="sxs-lookup"><span data-stu-id="b6916-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="b6916-158">Isso indica que há outras páginas de dados a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="b6916-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b6916-159">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="b6916-160">A resposta inclui o mesmo conjunto de propriedades que na solicitação de consulta Delta inicial.</span><span class="sxs-lookup"><span data-stu-id="b6916-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="b6916-161">Isso permite que você capture o estado atual completo dos objetos ao iniciar o ciclo Delta.</span><span class="sxs-lookup"><span data-stu-id="b6916-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="b6916-162">Se uma `deltaLink` URL for retornada:</span><span class="sxs-lookup"><span data-stu-id="b6916-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="b6916-163">Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b6916-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b6916-164">Salve e use a `deltaLink` URL para saber mais sobre as alterações no recurso na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="b6916-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="b6916-165">Você tem a opção de especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta somente para as propriedades que foram alteradas desde o momento `deltaLink` em que foi emitido.</span><span class="sxs-lookup"><span data-stu-id="b6916-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="b6916-166">Padrão: retornar as mesmas propriedades que a solicitação Delta inicial</span><span class="sxs-lookup"><span data-stu-id="b6916-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="b6916-167">Por padrão, as solicitações usando `deltaLink` uma `nextLink` ou retornam as mesmas propriedades selecionadas na consulta Delta inicial das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="b6916-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="b6916-168">Se a propriedade tiver sido alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b6916-169">Isso inclui propriedades que estão sendo definidas como valor nulo.</span><span class="sxs-lookup"><span data-stu-id="b6916-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b6916-170">Se a propriedade não tiver sido alterada, o valor antigo será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="b6916-171">Se a propriedade nunca tiver sido definida antes de não ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="b6916-172">**Observação:** Com esse comportamento, observando a resposta, não é possível dizer se uma propriedade está sendo alterada ou não.</span><span class="sxs-lookup"><span data-stu-id="b6916-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="b6916-173">Além disso, as respostas Delta tendem a ser grandes porque contêm todos os valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b6916-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="b6916-174">Alternativa: retornar somente as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="b6916-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="b6916-175">Adicionar um cabeçalho de solicitação opcional `prefer:return=minimal` --resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="b6916-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="b6916-176">Se a propriedade tiver sido alterada, o novo valor será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b6916-177">Isso inclui propriedades que estão sendo definidas como valor nulo.</span><span class="sxs-lookup"><span data-stu-id="b6916-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b6916-178">Se a propriedade não tiver sido alterada, a propriedade não será incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6916-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="b6916-179">(Diferente do comportamento padrão.)</span><span class="sxs-lookup"><span data-stu-id="b6916-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="b6916-180">**Observação:** O cabeçalho pode ser adicionado a uma `deltaLink` solicitação em um determinado momento no ciclo Delta.</span><span class="sxs-lookup"><span data-stu-id="b6916-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="b6916-181">O cabeçalho afeta apenas o conjunto de propriedades incluído na resposta e não afeta como a consulta Delta é executada.</span><span class="sxs-lookup"><span data-stu-id="b6916-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="b6916-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6916-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="b6916-183">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b6916-183">Request 1</span></span>

<span data-ttu-id="b6916-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6916-184">The following is an example of the request.</span></span> <span data-ttu-id="b6916-185">Não há nenhum `$select` parâmetro, portanto, um conjunto padrão de propriedades é rastreado e retornado.</span><span class="sxs-lookup"><span data-stu-id="b6916-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="b6916-186">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b6916-186">Response 1</span></span>

<span data-ttu-id="b6916-187">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="b6916-187">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b6916-188">Nenhum `isOf` filtro foi usado, portanto, todos os tipos derivados de directoryobject são retornados.</span><span class="sxs-lookup"><span data-stu-id="b6916-188">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="b6916-189">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6916-189">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6916-190">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6916-190">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",      
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="b6916-191">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b6916-191">Request 2</span></span>

<span data-ttu-id="b6916-192">O exemplo a seguir mostra o uso do comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="b6916-192">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="b6916-193">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b6916-193">Response 2</span></span>

<span data-ttu-id="b6916-194">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="b6916-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b6916-195">Observação apenas as propriedades que realmente foram alteradas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b6916-195">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="b6916-196">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="b6916-196">Request 3</span></span>

<span data-ttu-id="b6916-197">O próximo exemplo mostra a solicitação inicial usando o `isOf` operador para filtrar somente entidades de usuário e de Grupo:</span><span class="sxs-lookup"><span data-stu-id="b6916-197">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="b6916-198">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="b6916-198">Response 3</span></span>

<span data-ttu-id="b6916-199">Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.</span><span class="sxs-lookup"><span data-stu-id="b6916-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b6916-200">Observe que somente objetos de usuário e de grupo são retornados:</span><span class="sxs-lookup"><span data-stu-id="b6916-200">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- <span data-ttu-id="b6916-201">[Usar a consulta Delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b6916-201">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="b6916-202">[Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="b6916-202">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
