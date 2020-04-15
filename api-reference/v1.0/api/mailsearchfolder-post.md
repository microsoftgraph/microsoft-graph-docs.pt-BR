---
title: Criar mailSearchFolder
description: Use esta API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a3fa66ec626db22d995f268de72ced8d2c15b3c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43355228"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="79318-103">Criar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="79318-103">Create mailSearchFolder</span></span>

<span data-ttu-id="79318-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79318-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79318-105">Criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="79318-105">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="79318-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79318-106">Permissions</span></span>

<span data-ttu-id="79318-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79318-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79318-109">Permission type</span></span> | <span data-ttu-id="79318-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79318-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="79318-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79318-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79318-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79318-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79318-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79318-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79318-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79318-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79318-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79318-115">Application</span></span> | <span data-ttu-id="79318-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79318-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79318-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79318-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="79318-118">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="79318-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="79318-119">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="79318-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79318-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79318-120">Request headers</span></span>

| <span data-ttu-id="79318-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79318-121">Header</span></span> | <span data-ttu-id="79318-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79318-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="79318-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79318-123">Authorization</span></span> | <span data-ttu-id="79318-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="79318-124">`Bearer {token}`.</span></span> <span data-ttu-id="79318-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79318-125">Required.</span></span> |
| <span data-ttu-id="79318-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79318-126">Content-Type</span></span> | <span data-ttu-id="79318-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="79318-127">`application/json`.</span></span> <span data-ttu-id="79318-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79318-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79318-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79318-129">Request body</span></span>

<span data-ttu-id="79318-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79318-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79318-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="79318-131">Parameter</span></span> | <span data-ttu-id="79318-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="79318-132">Type</span></span> | <span data-ttu-id="79318-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="79318-133">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="79318-134">@odata.type</span><span class="sxs-lookup"><span data-stu-id="79318-134">@odata.type</span></span> | <span data-ttu-id="79318-135">String</span><span class="sxs-lookup"><span data-stu-id="79318-135">String</span></span> | <span data-ttu-id="79318-136">O tipo de pasta a ser criada.</span><span class="sxs-lookup"><span data-stu-id="79318-136">The type of folder to be created.</span></span> <span data-ttu-id="79318-137">Defina como "Microsoft. Graph. mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="79318-137">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="79318-138">displayName</span><span class="sxs-lookup"><span data-stu-id="79318-138">displayName</span></span> | <span data-ttu-id="79318-139">String</span><span class="sxs-lookup"><span data-stu-id="79318-139">String</span></span> | <span data-ttu-id="79318-140">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="79318-140">The display name of the new folder.</span></span>|
| <span data-ttu-id="79318-141">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="79318-141">includeNestedFolders</span></span> | <span data-ttu-id="79318-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="79318-142">Boolean</span></span> | <span data-ttu-id="79318-143">Indica como a hierarquia da pasta da caixa de correio deve ser percorrida na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="79318-143">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="79318-144">`true`significa que uma pesquisa profunda deve ser feita para incluir pastas filhas na hierarquia de cada pasta explicitamente especificada no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="79318-144">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="79318-145">`false`significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="79318-145">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="79318-146">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="79318-146">sourceFolderIds</span></span> | <span data-ttu-id="79318-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79318-147">String collection</span></span> | <span data-ttu-id="79318-148">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="79318-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="79318-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="79318-149">filterQuery</span></span> | <span data-ttu-id="79318-150">String</span><span class="sxs-lookup"><span data-stu-id="79318-150">String</span></span> | <span data-ttu-id="79318-151">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="79318-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="79318-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="79318-152">Response</span></span>

<span data-ttu-id="79318-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79318-153">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79318-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79318-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="79318-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79318-155">Request</span></span>

<span data-ttu-id="79318-156">Veja a seguir um exemplo de solicitação-ele cria uma pasta de pesquisa de mensagens que contêm a cadeia de caracteres "semanalmente Resumo" no assunto.</span><span class="sxs-lookup"><span data-stu-id="79318-156">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="79318-157">A pasta de pesquisa está na mesma pasta em que a consulta de filtro especificado se aplica.</span><span class="sxs-lookup"><span data-stu-id="79318-157">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="http"></a>[<span data-ttu-id="79318-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="79318-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```
# <a name="c"></a>[<span data-ttu-id="79318-159">C#</span><span class="sxs-lookup"><span data-stu-id="79318-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79318-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79318-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79318-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79318-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79318-162">Java</span><span class="sxs-lookup"><span data-stu-id="79318-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79318-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="79318-163">Response</span></span>

<span data-ttu-id="79318-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79318-164">The following is an example of the response.</span></span>

><span data-ttu-id="79318-165">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79318-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79318-166">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79318-166">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
}
```


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

  ]
}
-->
