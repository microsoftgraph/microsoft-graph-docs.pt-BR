---
title: 'directoryRole: delta'
description: Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Using Delta Query para obter detalhes.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 10a43389f9655409b4d00ecfbcece6687c66ff86
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118532"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="91bfb-104">directoryRole: delta</span><span class="sxs-lookup"><span data-stu-id="91bfb-104">directoryRole: delta</span></span>

<span data-ttu-id="91bfb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bfb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91bfb-106">Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="91bfb-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="91bfb-107">Consulte [Using Delta Query](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="91bfb-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="91bfb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="91bfb-108">Permissions</span></span>

<span data-ttu-id="91bfb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bfb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91bfb-111">Permission type</span></span>      | <span data-ttu-id="91bfb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91bfb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91bfb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91bfb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91bfb-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91bfb-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91bfb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91bfb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91bfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91bfb-116">Not supported.</span></span>    |
|<span data-ttu-id="91bfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91bfb-117">Application</span></span> | <span data-ttu-id="91bfb-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91bfb-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91bfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91bfb-119">HTTP request</span></span>

<span data-ttu-id="91bfb-120">Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso directoryRole.</span><span class="sxs-lookup"><span data-stu-id="91bfb-120">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http

GET /directoryRoles/delta

```

### <a name="query-parameters"></a><span data-ttu-id="91bfb-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="91bfb-121">Query parameters</span></span>

<span data-ttu-id="91bfb-122">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="91bfb-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="91bfb-123">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="91bfb-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="91bfb-124">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfb-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="91bfb-125">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="91bfb-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="91bfb-126">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="91bfb-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="91bfb-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="91bfb-127">Query parameter</span></span>      | <span data-ttu-id="91bfb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="91bfb-128">Type</span></span>   |<span data-ttu-id="91bfb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bfb-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91bfb-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="91bfb-130">$deltatoken</span></span> | <span data-ttu-id="91bfb-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfb-131">string</span></span> | <span data-ttu-id="91bfb-132">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="91bfb-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="91bfb-133">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="91bfb-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="91bfb-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="91bfb-134">$skiptoken</span></span> | <span data-ttu-id="91bfb-135">string</span><span class="sxs-lookup"><span data-stu-id="91bfb-135">string</span></span> | <span data-ttu-id="91bfb-136">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="91bfb-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="91bfb-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91bfb-137">Optional query parameters</span></span>

<span data-ttu-id="91bfb-138">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfb-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="91bfb-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="91bfb-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="91bfb-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="91bfb-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="91bfb-142">A única expressão `$filter` com suporte é para controlar alterações para recursos específicos, por sua id: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="91bfb-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="91bfb-143">O número de ids que você pode especificar é limitado pelo tamanho máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="91bfb-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="91bfb-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfb-144">Request headers</span></span>
| <span data-ttu-id="91bfb-145">Nome</span><span class="sxs-lookup"><span data-stu-id="91bfb-145">Name</span></span>       | <span data-ttu-id="91bfb-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bfb-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91bfb-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="91bfb-147">Authorization</span></span>  | <span data-ttu-id="91bfb-148">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="91bfb-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="91bfb-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91bfb-149">Content-Type</span></span>  | <span data-ttu-id="91bfb-150">application/json</span><span class="sxs-lookup"><span data-stu-id="91bfb-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="91bfb-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfb-151">Request body</span></span>
<span data-ttu-id="91bfb-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91bfb-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="91bfb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfb-153">Response</span></span>

<span data-ttu-id="91bfb-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto da coleção directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfb-154">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="91bfb-155">A resposta também inclui uma URL do nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="91bfb-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="91bfb-156">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="91bfb-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="91bfb-157">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfb-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="91bfb-158">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="91bfb-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="91bfb-159">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="91bfb-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="91bfb-160">Confira:</span><span class="sxs-lookup"><span data-stu-id="91bfb-160">See:</span></span></br>
- <span data-ttu-id="91bfb-161">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="91bfb-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="91bfb-162">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="91bfb-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="91bfb-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91bfb-163">Example</span></span>
#### <a name="request"></a><span data-ttu-id="91bfb-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfb-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="91bfb-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="91bfb-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="91bfb-166">C#</span><span class="sxs-lookup"><span data-stu-id="91bfb-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91bfb-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91bfb-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91bfb-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91bfb-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91bfb-169">Java</span><span class="sxs-lookup"><span data-stu-id="91bfb-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91bfb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfb-170">Response</span></span>
><span data-ttu-id="91bfb-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="91bfb-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink": "https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pkXMyA5aFCIMmH1Kk1XEAnf2X-fodqXKXF03gYPQknSHRxogVsxvSq_26nhos-O2-shortened",
  "value": [
    {
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8",
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "members@delta": [
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "bb165b45-151c-4cf6-9911-cd7188912848",
          "@removed": {
            "reason": "deleted"
          }
        }
      ]
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


