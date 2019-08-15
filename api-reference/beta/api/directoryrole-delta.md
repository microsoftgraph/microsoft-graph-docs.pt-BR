---
title: 'directoryRole: Delta'
description: Obter funções de diretório recém-criadas, atualizadas ou excluídas sem ter que executar uma leitura completa de toda a coleção de recursos. Consulte usando a consulta Delta para obter detalhes.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7941c3de313c7d16681e3eb26b36b6ab59243aaf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417309"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="0b70b-104">directoryRole: Delta</span><span class="sxs-lookup"><span data-stu-id="0b70b-104">directoryRole: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b70b-105">Obter funções de diretório recém-criadas, atualizadas ou excluídas sem ter que executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="0b70b-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="0b70b-106">Consulte [usando a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="0b70b-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b70b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b70b-107">Permissions</span></span>

<span data-ttu-id="0b70b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b70b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b70b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b70b-110">Permission type</span></span>      | <span data-ttu-id="0b70b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b70b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b70b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b70b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b70b-113">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="0b70b-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b70b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b70b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b70b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b70b-115">Not supported.</span></span>    |
|<span data-ttu-id="0b70b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b70b-116">Application</span></span> | <span data-ttu-id="0b70b-117">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0b70b-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b70b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b70b-118">HTTP request</span></span>

<span data-ttu-id="0b70b-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso directoryRole.</span><span class="sxs-lookup"><span data-stu-id="0b70b-119">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http

GET /directoryRoles/delta

```

### <a name="query-parameters"></a><span data-ttu-id="0b70b-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="0b70b-120">Query parameters</span></span>

<span data-ttu-id="0b70b-121">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="0b70b-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="0b70b-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="0b70b-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="0b70b-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="0b70b-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="0b70b-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="0b70b-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="0b70b-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="0b70b-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="0b70b-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="0b70b-126">Query parameter</span></span>      | <span data-ttu-id="0b70b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b70b-127">Type</span></span>   |<span data-ttu-id="0b70b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b70b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b70b-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="0b70b-129">$deltatoken</span></span> | <span data-ttu-id="0b70b-130">string</span><span class="sxs-lookup"><span data-stu-id="0b70b-130">string</span></span> | <span data-ttu-id="0b70b-131">Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="0b70b-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="0b70b-132">Salve e aplique a URL `deltaLink` inteira incluindo esse token na primeira solicitação da próxima rodada de controle de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="0b70b-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="0b70b-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0b70b-133">$skiptoken</span></span> | <span data-ttu-id="0b70b-134">string</span><span class="sxs-lookup"><span data-stu-id="0b70b-134">string</span></span> | <span data-ttu-id="0b70b-135">Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="0b70b-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="0b70b-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b70b-136">Optional query parameters</span></span>

<span data-ttu-id="0b70b-137">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b70b-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="0b70b-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="0b70b-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="0b70b-140">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="0b70b-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="0b70b-141">A única expressão `$filter` suportada é para controlar alterações de recursos específicos, por sua `$filter=id+eq+{value}` ID `$filter=id+eq+{value1}+or+id+eq+{value2}`: ou.</span><span class="sxs-lookup"><span data-stu-id="0b70b-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="0b70b-142">O número de IDs que você pode especificar é limitado pelo tamanho máximo de URL.</span><span class="sxs-lookup"><span data-stu-id="0b70b-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="0b70b-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b70b-143">Request headers</span></span>
| <span data-ttu-id="0b70b-144">Nome</span><span class="sxs-lookup"><span data-stu-id="0b70b-144">Name</span></span>       | <span data-ttu-id="0b70b-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b70b-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b70b-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b70b-146">Authorization</span></span>  | <span data-ttu-id="0b70b-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="0b70b-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="0b70b-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b70b-148">Content-Type</span></span>  | <span data-ttu-id="0b70b-149">application/json</span><span class="sxs-lookup"><span data-stu-id="0b70b-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b70b-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b70b-150">Request body</span></span>
<span data-ttu-id="0b70b-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b70b-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="0b70b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b70b-152">Response</span></span>

<span data-ttu-id="0b70b-153">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b70b-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="0b70b-154">A resposta também inclui uma URL do nextLink ou uma URL do deltaLink.</span><span class="sxs-lookup"><span data-stu-id="0b70b-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="0b70b-155">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="0b70b-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="0b70b-156">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="0b70b-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="0b70b-157">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="0b70b-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="0b70b-158">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="0b70b-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="0b70b-159">Confira:</span><span class="sxs-lookup"><span data-stu-id="0b70b-159">See:</span></span></br>
- <span data-ttu-id="0b70b-160">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0b70b-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="0b70b-161">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="0b70b-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="0b70b-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b70b-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b70b-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b70b-163">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b70b-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b70b-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b70b-165">C#</span><span class="sxs-lookup"><span data-stu-id="0b70b-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b70b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b70b-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b70b-167">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b70b-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0b70b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b70b-168">Response</span></span>
<span data-ttu-id="0b70b-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b70b-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
