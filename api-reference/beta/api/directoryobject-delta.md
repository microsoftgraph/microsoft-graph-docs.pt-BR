---
title: 'directoryObject: delta'
description: 'Get recentemente criado, atualizado ou excluído objetos de diretório dos seguintes tipos: usuário, grupo e contato organizacional, em uma consulta delta único. Consulte controlar alterações para obter detalhes.'
localization_priority: Normal
ms.openlocfilehash: 823107bce56d77c4e9c29a77405ac014443f5190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854492"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="6dc98-104">directoryObject: delta</span><span class="sxs-lookup"><span data-stu-id="6dc98-104">directoryObject: delta</span></span>

> <span data-ttu-id="6dc98-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6dc98-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dc98-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6dc98-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dc98-107">Get recentemente criado, atualizado ou excluído objetos de diretório dos seguintes tipos: [usuário](../resources/user.md), [grupo](../resources/group.md) e [contato organizacional](../resources/orgcontact.md), em uma consulta delta único.</span><span class="sxs-lookup"><span data-stu-id="6dc98-107">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="6dc98-108">Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="6dc98-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc98-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="6dc98-109">Permissions</span></span>

<span data-ttu-id="6dc98-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc98-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc98-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dc98-112">Permission type</span></span>      | <span data-ttu-id="6dc98-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dc98-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dc98-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dc98-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6dc98-115">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dc98-115">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="6dc98-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dc98-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dc98-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dc98-117">Not supported.</span></span>  |
|<span data-ttu-id="6dc98-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dc98-118">Application</span></span> | <span data-ttu-id="6dc98-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc98-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dc98-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dc98-120">HTTP request</span></span>

<span data-ttu-id="6dc98-121">Para começar a controlar alterações, você deve fazer uma solicitação, incluindo a função delta no recurso directoryObjects.</span><span class="sxs-lookup"><span data-stu-id="6dc98-121">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="6dc98-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="6dc98-122">Query parameters</span></span>

<span data-ttu-id="6dc98-123">Controle de alterações provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="6dc98-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="6dc98-124">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="6dc98-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="6dc98-125">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="6dc98-126">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="6dc98-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="6dc98-127">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="6dc98-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="6dc98-128">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="6dc98-128">Query parameter</span></span> | <span data-ttu-id="6dc98-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc98-129">Type</span></span> |<span data-ttu-id="6dc98-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc98-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6dc98-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="6dc98-131">$deltatoken</span></span> | <span data-ttu-id="6dc98-132">string</span><span class="sxs-lookup"><span data-stu-id="6dc98-132">string</span></span> | <span data-ttu-id="6dc98-p106">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="6dc98-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="6dc98-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="6dc98-135">$skiptoken</span></span> | <span data-ttu-id="6dc98-136">string</span><span class="sxs-lookup"><span data-stu-id="6dc98-136">string</span></span> | <span data-ttu-id="6dc98-137">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="6dc98-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="6dc98-138">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="6dc98-138">OData query parameters</span></span>

<span data-ttu-id="6dc98-139">Este método oferece suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="6dc98-140">Você pode usar `$filter` com o especial `isOf` operador para filtrar um subconjunto dos tipos derivados directoryObject.</span><span class="sxs-lookup"><span data-stu-id="6dc98-140">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="6dc98-141">Você pode combinar várias expressões usando um `or`, que permite que você tiver uma consulta única delta vários tipos de acompanhamento.</span><span class="sxs-lookup"><span data-stu-id="6dc98-141">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="6dc98-142">Consulte o [terceiro exemplo](#request-3) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="6dc98-142">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dc98-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc98-143">Request headers</span></span>

| <span data-ttu-id="6dc98-144">Nome</span><span class="sxs-lookup"><span data-stu-id="6dc98-144">Name</span></span>       | <span data-ttu-id="6dc98-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc98-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6dc98-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dc98-146">Authorization</span></span>  | <span data-ttu-id="6dc98-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="6dc98-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="6dc98-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dc98-148">Content-Type</span></span>  | <span data-ttu-id="6dc98-149">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc98-149">application/json</span></span> |
| <span data-ttu-id="6dc98-150">Preferir</span><span class="sxs-lookup"><span data-stu-id="6dc98-150">Prefer</span></span> | <span data-ttu-id="6dc98-151">retornar = mínima</span><span class="sxs-lookup"><span data-stu-id="6dc98-151">return=minimal</span></span> <br><br><span data-ttu-id="6dc98-152">Especificando este cabeçalho com uma solicitação que usa um `deltaLink` retornaria apenas as propriedades do objeto que foram alterados desde o último round.</span><span class="sxs-lookup"><span data-stu-id="6dc98-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="6dc98-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6dc98-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dc98-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc98-154">Request body</span></span>

<span data-ttu-id="6dc98-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6dc98-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6dc98-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dc98-156">Response</span></span>

<span data-ttu-id="6dc98-157">Se tiver êxito, este método retornará `200 OK` objeto de coleção [usuário](../resources/directoryobject.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-157">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="6dc98-158">A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="6dc98-158">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="6dc98-159">Se um `nextLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="6dc98-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="6dc98-160">Isso indica que há páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="6dc98-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="6dc98-161">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="6dc98-162">A resposta inclui o mesmo conjunto de propriedades que a solicitação de consulta inicial delta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="6dc98-163">Isso permite que você capture o estado atual completa dos objetos ao iniciar o ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="6dc98-164">Se um `deltaLink` URL é retornado:</span><span class="sxs-lookup"><span data-stu-id="6dc98-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="6dc98-165">Isso indica que não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6dc98-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="6dc98-166">Salvar e utilizar o `deltaLink` para saber mais sobre a URL é alterada para o recurso na próxima fase.</span><span class="sxs-lookup"><span data-stu-id="6dc98-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="6dc98-167">Você tem uma escolha para especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta para apenas as propriedades que foram alterados desde o momento de `deltaLink` foi emitido.</span><span class="sxs-lookup"><span data-stu-id="6dc98-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="6dc98-168">Padrão: retornar as mesmas propriedades que a solicitação inicial delta</span><span class="sxs-lookup"><span data-stu-id="6dc98-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="6dc98-169">Por padrão, as solicitações usando um `deltaLink` ou `nextLink` retornar as mesmas propriedades selecionado na consulta inicial delta das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="6dc98-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="6dc98-170">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-170">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6dc98-171">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="6dc98-171">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6dc98-172">Se a propriedade não tiver sido alterado, o valor antigo está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-172">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="6dc98-173">Se a propriedade nunca tiver sido definida antes que ele não será incluído na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="6dc98-173">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="6dc98-174">**Observação:** Com esse comportamento, examinando a resposta não é possível saber se uma propriedade está mudando ou não.</span><span class="sxs-lookup"><span data-stu-id="6dc98-174">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="6dc98-175">Além disso, as respostas delta tendem a ser grandes porque eles contêm todos os valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6dc98-175">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="6dc98-176">Alternativa: retornar apenas as propriedades alteradas</span><span class="sxs-lookup"><span data-stu-id="6dc98-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="6dc98-177">Adicionando um cabeçalho de solicitação opcionais - `prefer:return=minimal` -resulta no seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="6dc98-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="6dc98-178">Se a propriedade foi alterada, o novo valor é incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-178">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6dc98-179">Isso inclui propriedades sendo definidas como um valor nulo.</span><span class="sxs-lookup"><span data-stu-id="6dc98-179">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6dc98-180">Se a propriedade não tiver sido alterado, a propriedade não está incluída na resposta nisso.</span><span class="sxs-lookup"><span data-stu-id="6dc98-180">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="6dc98-181">(Diferente do comportamento padrão).</span><span class="sxs-lookup"><span data-stu-id="6dc98-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="6dc98-182">**Observação:** O cabeçalho pode ser adicionado a um `deltaLink` solicitação a qualquer momento no ciclo de delta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="6dc98-183">O cabeçalho afeta somente o conjunto de propriedades incluído na resposta e ela não afeta como a consulta de delta é executada.</span><span class="sxs-lookup"><span data-stu-id="6dc98-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="6dc98-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dc98-184">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="6dc98-185">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="6dc98-185">Request 1</span></span>

<span data-ttu-id="6dc98-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dc98-186">The following is an example of the request.</span></span> <span data-ttu-id="6dc98-187">Não há nenhum `$select` parâmetro, para que um conjunto de propriedades padrão é controlado e retornado.</span><span class="sxs-lookup"><span data-stu-id="6dc98-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="6dc98-188">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="6dc98-188">Response 1</span></span>

<span data-ttu-id="6dc98-189">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6dc98-190">Não `isOf` filtro tiver sido usado, portanto, todos os tipos derivados de directoryObject são retornados.</span><span class="sxs-lookup"><span data-stu-id="6dc98-190">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="6dc98-p120">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dc98-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
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
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="6dc98-193">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="6dc98-193">Request 2</span></span>

<span data-ttu-id="6dc98-194">O exemplo a seguir mostra o uso do comportamento de resposta mínimo alternativo:</span><span class="sxs-lookup"><span data-stu-id="6dc98-194">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="6dc98-195">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="6dc98-195">Response 2</span></span>

<span data-ttu-id="6dc98-196">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6dc98-197">Observe que apenas as propriedades que foram alterados, na verdade, são retornadas.</span><span class="sxs-lookup"><span data-stu-id="6dc98-197">Note only the properties that have actually changed are returned.</span></span>

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
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="6dc98-198">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="6dc98-198">Request 3</span></span>

<span data-ttu-id="6dc98-199">O exemplo a seguir mostra a solicitação inicial usando o `isOf` operador para filtrar somente entidades de usuário e de grupo:</span><span class="sxs-lookup"><span data-stu-id="6dc98-199">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="6dc98-200">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="6dc98-200">Response 3</span></span>

<span data-ttu-id="6dc98-201">A seguir está um exemplo da resposta ao usar `deltaLink` obtido a inicialização de consulta.</span><span class="sxs-lookup"><span data-stu-id="6dc98-201">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6dc98-202">Observe que apenas os objetos de usuário e de grupo são retornados:</span><span class="sxs-lookup"><span data-stu-id="6dc98-202">Note that only user and group objects are returned:</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- <span data-ttu-id="6dc98-203">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="6dc98-203">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="6dc98-204">[Fazer alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="6dc98-204">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
