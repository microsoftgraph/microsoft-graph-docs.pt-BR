---
title: Criar mailSearchFolder
description: Use esta API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c600048961b560364982b8b8ef5cff531ae2031
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598205"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="a5427-103">Criar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="a5427-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5427-104">Use esta API para criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="a5427-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5427-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5427-105">Permissions</span></span>

<span data-ttu-id="a5427-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5427-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5427-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5427-108">Permission type</span></span> | <span data-ttu-id="a5427-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5427-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a5427-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5427-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5427-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5427-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5427-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5427-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5427-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5427-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5427-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5427-114">Application</span></span> | <span data-ttu-id="a5427-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5427-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5427-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5427-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="a5427-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="a5427-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="a5427-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a5427-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5427-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5427-119">Request headers</span></span>

| <span data-ttu-id="a5427-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5427-120">Header</span></span> | <span data-ttu-id="a5427-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a5427-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a5427-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5427-122">Authorization</span></span> | <span data-ttu-id="a5427-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a5427-123"></span></span> <span data-ttu-id="a5427-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5427-124">Required.</span></span> |
| <span data-ttu-id="a5427-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5427-125">Content-Type</span></span> | <span data-ttu-id="a5427-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a5427-126"></span></span> <span data-ttu-id="a5427-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5427-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5427-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5427-128">Request body</span></span>

<span data-ttu-id="a5427-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5427-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a5427-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a5427-130">Parameter</span></span> | <span data-ttu-id="a5427-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5427-131">Type</span></span> | <span data-ttu-id="a5427-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5427-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a5427-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="a5427-133">@odata.type</span></span> | <span data-ttu-id="a5427-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5427-134">String</span></span> | <span data-ttu-id="a5427-135">O tipo de pasta a ser criada.</span><span class="sxs-lookup"><span data-stu-id="a5427-135">The type of folder to be created.</span></span> <span data-ttu-id="a5427-136">Defina como "Microsoft. Graph. mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="a5427-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="a5427-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a5427-137">displayName</span></span> | <span data-ttu-id="a5427-138">String</span><span class="sxs-lookup"><span data-stu-id="a5427-138">String</span></span> | <span data-ttu-id="a5427-139">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="a5427-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="a5427-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="a5427-140">includeNestedFolders</span></span> | <span data-ttu-id="a5427-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5427-141">Boolean</span></span> | <span data-ttu-id="a5427-142">Como a hierarquia da pasta de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="a5427-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="a5427-143">`true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada.</span><span class="sxs-lookup"><span data-stu-id="a5427-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="a5427-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="a5427-144">sourceFolderIDs</span></span> | <span data-ttu-id="a5427-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5427-145">String collection</span></span> | <span data-ttu-id="a5427-146">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="a5427-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="a5427-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="a5427-147">filterQuery</span></span> | <span data-ttu-id="a5427-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5427-148">String</span></span> | <span data-ttu-id="a5427-149">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="a5427-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="a5427-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5427-150">Response</span></span>

<span data-ttu-id="a5427-151">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5427-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5427-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5427-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a5427-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5427-153">Request</span></span>

<span data-ttu-id="a5427-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5427-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="a5427-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5427-155">Response</span></span>

<span data-ttu-id="a5427-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5427-156">The following is an example of the response.</span></span>

><span data-ttu-id="a5427-157">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5427-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5427-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5427-158">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5427-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a5427-159">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5427-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5427-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailsearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
