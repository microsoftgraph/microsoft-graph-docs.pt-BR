---
title: Atualizar mailSearchFolder
description: Atualizar as propriedades graváveis de um objeto mailSearchFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fc013c5fc8096f1d567a41c066c788159cab9a81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449810"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="24feb-103">Atualizar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="24feb-103">Update mailSearchFolder</span></span>

<span data-ttu-id="24feb-104">Atualizar as propriedades graváveis de um objeto [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="24feb-104">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24feb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24feb-105">Permissions</span></span>
<span data-ttu-id="24feb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24feb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24feb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24feb-108">Permission type</span></span>      | <span data-ttu-id="24feb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24feb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24feb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24feb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24feb-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24feb-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="24feb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24feb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24feb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24feb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="24feb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24feb-114">Application</span></span> | <span data-ttu-id="24feb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24feb-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="24feb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24feb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="24feb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-117">Request headers</span></span>
| <span data-ttu-id="24feb-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24feb-118">Header</span></span>       | <span data-ttu-id="24feb-119">Valor</span><span class="sxs-lookup"><span data-stu-id="24feb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24feb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="24feb-120">Authorization</span></span>  | <span data-ttu-id="24feb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24feb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="24feb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24feb-123">Content-Type</span></span>  | <span data-ttu-id="24feb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24feb-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24feb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-126">Request body</span></span>
<span data-ttu-id="24feb-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="24feb-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="24feb-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="24feb-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="24feb-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="24feb-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="24feb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24feb-130">Property</span></span>     | <span data-ttu-id="24feb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="24feb-131">Type</span></span>   |<span data-ttu-id="24feb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="24feb-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24feb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="24feb-133">displayName</span></span> | <span data-ttu-id="24feb-134">String</span><span class="sxs-lookup"><span data-stu-id="24feb-134">String</span></span> | <span data-ttu-id="24feb-135">O nome de exibição do [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="24feb-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="24feb-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="24feb-136">includeNestedFolders</span></span> | <span data-ttu-id="24feb-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="24feb-137">Boolean</span></span> | <span data-ttu-id="24feb-138">Como a hierarquia da pasta de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="24feb-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="24feb-139">`true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada.</span><span class="sxs-lookup"><span data-stu-id="24feb-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="24feb-140">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="24feb-140">sourceFolderIds</span></span> | <span data-ttu-id="24feb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="24feb-141">String collection</span></span> | <span data-ttu-id="24feb-142">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="24feb-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="24feb-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="24feb-143">filterQuery</span></span> | <span data-ttu-id="24feb-144">String</span><span class="sxs-lookup"><span data-stu-id="24feb-144">String</span></span> | <span data-ttu-id="24feb-145">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="24feb-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="24feb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="24feb-146">Response</span></span>
<span data-ttu-id="24feb-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24feb-147">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24feb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24feb-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="24feb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-149">Request</span></span>
<span data-ttu-id="24feb-150">A seguir está um exemplo de solicitação que atualiza a propriedade **filterQuery** da pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="24feb-150">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24feb-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="24feb-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24feb-152">C#</span><span class="sxs-lookup"><span data-stu-id="24feb-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24feb-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="24feb-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24feb-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="24feb-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24feb-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="24feb-155">Response</span></span>
<span data-ttu-id="24feb-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24feb-156">The following is an example of the response.</span></span>
><span data-ttu-id="24feb-157">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24feb-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24feb-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24feb-158">All the properties will be returned from an actual call.</span></span>
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
