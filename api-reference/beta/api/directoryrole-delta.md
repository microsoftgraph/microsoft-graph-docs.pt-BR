---
title: 'directoryRole: delta'
description: Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Using Delta Query para obter detalhes.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8ab916a6808422624ba511ad728100b315156be7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436817"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="28d20-104">directoryRole: delta</span><span class="sxs-lookup"><span data-stu-id="28d20-104">directoryRole: delta</span></span>

<span data-ttu-id="28d20-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d20-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d20-106">Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="28d20-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="28d20-107">Consulte [Using Delta Query](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="28d20-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="28d20-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="28d20-108">Permissions</span></span>

<span data-ttu-id="28d20-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d20-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d20-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28d20-111">Permission type</span></span>      | <span data-ttu-id="28d20-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28d20-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28d20-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28d20-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28d20-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28d20-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28d20-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28d20-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28d20-116">Not supported.</span></span>    |
|<span data-ttu-id="28d20-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28d20-117">Application</span></span> | <span data-ttu-id="28d20-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d20-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28d20-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28d20-119">HTTP request</span></span>

<span data-ttu-id="28d20-120">Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso directoryRole.</span><span class="sxs-lookup"><span data-stu-id="28d20-120">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http

GET /directoryRoles/delta

```

### <a name="query-parameters"></a><span data-ttu-id="28d20-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="28d20-121">Query parameters</span></span>

<span data-ttu-id="28d20-122">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="28d20-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="28d20-123">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="28d20-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="28d20-124">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="28d20-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="28d20-125">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="28d20-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="28d20-126">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="28d20-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="28d20-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="28d20-127">Query parameter</span></span>      | <span data-ttu-id="28d20-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="28d20-128">Type</span></span>   |<span data-ttu-id="28d20-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="28d20-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28d20-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="28d20-130">$deltatoken</span></span> | <span data-ttu-id="28d20-131">string</span><span class="sxs-lookup"><span data-stu-id="28d20-131">string</span></span> | <span data-ttu-id="28d20-132">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="28d20-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="28d20-133">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="28d20-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="28d20-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="28d20-134">$skiptoken</span></span> | <span data-ttu-id="28d20-135">string</span><span class="sxs-lookup"><span data-stu-id="28d20-135">string</span></span> | <span data-ttu-id="28d20-136">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="28d20-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="28d20-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28d20-137">Optional query parameters</span></span>

<span data-ttu-id="28d20-138">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28d20-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="28d20-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="28d20-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="28d20-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="28d20-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="28d20-142">A única expressão `$filter` com suporte é para controlar alterações para recursos específicos, por sua id: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="28d20-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="28d20-143">O número de ids que você pode especificar é limitado pelo tamanho máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="28d20-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="28d20-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28d20-144">Request headers</span></span>
| <span data-ttu-id="28d20-145">Nome</span><span class="sxs-lookup"><span data-stu-id="28d20-145">Name</span></span>       | <span data-ttu-id="28d20-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="28d20-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28d20-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="28d20-147">Authorization</span></span>  | <span data-ttu-id="28d20-148">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="28d20-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="28d20-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28d20-149">Content-Type</span></span>  | <span data-ttu-id="28d20-150">application/json</span><span class="sxs-lookup"><span data-stu-id="28d20-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="28d20-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28d20-151">Request body</span></span>
<span data-ttu-id="28d20-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28d20-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="28d20-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d20-153">Response</span></span>

<span data-ttu-id="28d20-154">Se tiver êxito, este método retornará o código de resposta e o `200 OK` [objeto da coleção directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28d20-154">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="28d20-155">A resposta também inclui uma URL do nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="28d20-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="28d20-156">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="28d20-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="28d20-157">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="28d20-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="28d20-158">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="28d20-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="28d20-159">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="28d20-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="28d20-160">Confira:</span><span class="sxs-lookup"><span data-stu-id="28d20-160">See:</span></span></br>
- <span data-ttu-id="28d20-161">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="28d20-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="28d20-162">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="28d20-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="28d20-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28d20-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28d20-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d20-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="28d20-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="28d20-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="28d20-166">C#</span><span class="sxs-lookup"><span data-stu-id="28d20-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28d20-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28d20-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28d20-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28d20-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28d20-169">Java</span><span class="sxs-lookup"><span data-stu-id="28d20-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="28d20-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d20-170">Response</span></span>
<span data-ttu-id="28d20-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28d20-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


