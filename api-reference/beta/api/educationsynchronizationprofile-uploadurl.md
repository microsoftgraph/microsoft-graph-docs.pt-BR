---
title: 'educationSynchronizationProfile: uploadUrl'
description: Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem no armazenamento de blob do Azure para um perfil específico de sincronização de dados escolares no locatário. O token SAS tem uma validade de uma hora.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d8a8a7f1cfd01ed63b54b66d888b3eb9e80d3a30
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664710"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="f5c4c-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="f5c4c-104">educationSynchronizationProfile: uploadUrl</span></span>

<span data-ttu-id="f5c4c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5c4c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c4c-106">Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem no armazenamento de blob do Azure para um perfil específico de sincronização de dados escolares no locatário. [](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-106">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f5c4c-107">O token SAS tem uma validade de uma hora.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-107">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="f5c4c-108">A URL de carregamento é fornecida apenas para o provedor de dados [CSV.](../resources/educationcsvdataprovider.md)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-108">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="f5c4c-109">**Observação:** Para acessar o armazenamento de blob com o token SAS, use os [SDKs](https://github.com/search?q=org%3AAzure+azure-storage) de armazenamento do Azure ou [o AzCopy](/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="f5c4c-109">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c4c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5c4c-110">Permissions</span></span>
<span data-ttu-id="f5c4c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5c4c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5c4c-113">Permission type</span></span> | <span data-ttu-id="f5c4c-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5c4c-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f5c4c-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c4c-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5c4c-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f5c4c-117">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f5c4c-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f5c4c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-118">Not supported.</span></span>|
|<span data-ttu-id="f5c4c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c4c-119">Application</span></span>|<span data-ttu-id="f5c4c-120">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5c4c-120">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5c4c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c4c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="f5c4c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c4c-122">Request headers</span></span>
| <span data-ttu-id="f5c4c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f5c4c-123">Name</span></span>       | <span data-ttu-id="f5c4c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5c4c-124">Type</span></span> | <span data-ttu-id="f5c4c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c4c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5c4c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c4c-126">Authorization</span></span>  | <span data-ttu-id="f5c4c-127">string</span><span class="sxs-lookup"><span data-stu-id="f5c4c-127">string</span></span>  | <span data-ttu-id="f5c4c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5c4c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c4c-130">Request body</span></span>
<span data-ttu-id="f5c4c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f5c4c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c4c-132">Response</span></span>
<span data-ttu-id="f5c4c-133">Se tiver êxito, este método retornará um código de resposta e uma URL SAS para `200 OK` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-133">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="f5c4c-134">Se uma solicitação anterior ainda estiver sendo processada, este método retornará um indicando que o carregamento está bloqueado no momento para `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f5c4c-134">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="f5c4c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5c4c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5c4c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c4c-136">Request</span></span>
<span data-ttu-id="f5c4c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5c4c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c4c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="c"></a>[<span data-ttu-id="f5c4c-139">C#</span><span class="sxs-lookup"><span data-stu-id="f5c4c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5c4c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5c4c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5c4c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5c4c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5c4c-142">Java</span><span class="sxs-lookup"><span data-stu-id="f5c4c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5c4c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c4c-143">Response</span></span>
<span data-ttu-id="f5c4c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-144">The following is an example of the response.</span></span>

><span data-ttu-id="f5c4c-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


