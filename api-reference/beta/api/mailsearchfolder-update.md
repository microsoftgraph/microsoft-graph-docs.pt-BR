---
title: Atualizar mailSearchFolder
description: Atualize as propriedades graváveis do objeto mailSearchFolder.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 711b5eeaea28b2dd5ec29eacf092780295377092
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981620"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="e7d38-103">Atualizar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="e7d38-103">Update mailSearchFolder</span></span>

<span data-ttu-id="e7d38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d38-105">Atualizar as propriedades graváveis de um objeto [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="e7d38-105">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d38-106">Permissions</span></span>
<span data-ttu-id="e7d38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d38-109">Permission type</span></span>      | <span data-ttu-id="e7d38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7d38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7d38-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d38-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d38-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e7d38-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d38-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d38-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e7d38-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d38-115">Application</span></span> | <span data-ttu-id="e7d38-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d38-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7d38-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d38-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7d38-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d38-118">Request headers</span></span>
| <span data-ttu-id="e7d38-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7d38-119">Header</span></span>       | <span data-ttu-id="e7d38-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e7d38-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7d38-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d38-121">Authorization</span></span>  | <span data-ttu-id="e7d38-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d38-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e7d38-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7d38-124">Content-Type</span></span>  | <span data-ttu-id="e7d38-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d38-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7d38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d38-127">Request body</span></span>
<span data-ttu-id="e7d38-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e7d38-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e7d38-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e7d38-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e7d38-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e7d38-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e7d38-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7d38-131">Property</span></span>     | <span data-ttu-id="e7d38-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7d38-132">Type</span></span>   |<span data-ttu-id="e7d38-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d38-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7d38-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e7d38-134">displayName</span></span> | <span data-ttu-id="e7d38-135">String</span><span class="sxs-lookup"><span data-stu-id="e7d38-135">String</span></span> | <span data-ttu-id="e7d38-136">O nome de exibição do [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e7d38-136">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="e7d38-137">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="e7d38-137">includeNestedFolders</span></span> | <span data-ttu-id="e7d38-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7d38-138">Boolean</span></span> | <span data-ttu-id="e7d38-139">Como a hierarquia da pasta de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="e7d38-139">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="e7d38-140">`true` significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada.</span><span class="sxs-lookup"><span data-stu-id="e7d38-140">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="e7d38-141">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="e7d38-141">sourceFolderIds</span></span> | <span data-ttu-id="e7d38-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d38-142">String collection</span></span> | <span data-ttu-id="e7d38-143">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="e7d38-143">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="e7d38-144">filterQuery</span><span class="sxs-lookup"><span data-stu-id="e7d38-144">filterQuery</span></span> | <span data-ttu-id="e7d38-145">String</span><span class="sxs-lookup"><span data-stu-id="e7d38-145">String</span></span> | <span data-ttu-id="e7d38-146">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="e7d38-146">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="e7d38-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d38-147">Response</span></span>
<span data-ttu-id="e7d38-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d38-148">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7d38-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d38-149">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e7d38-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d38-150">Request</span></span>
<span data-ttu-id="e7d38-151">A seguir está um exemplo de solicitação que atualiza a propriedade **filterQuery** da pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e7d38-151">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7d38-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d38-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```
# <a name="c"></a>[<span data-ttu-id="e7d38-153">C#</span><span class="sxs-lookup"><span data-stu-id="e7d38-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7d38-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7d38-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7d38-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7d38-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7d38-156">Java</span><span class="sxs-lookup"><span data-stu-id="e7d38-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7d38-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d38-157">Response</span></span>
<span data-ttu-id="e7d38-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d38-158">The following is an example of the response.</span></span>
><span data-ttu-id="e7d38-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d38-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


