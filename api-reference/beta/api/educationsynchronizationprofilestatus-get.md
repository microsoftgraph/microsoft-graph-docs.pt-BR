---
title: Obter o status de um educationSynchronizationProfile
description: Obter o status de um perfil de sincronização de dados escolar específico no locatário. A resposta indicará o status da sincronização.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7bc697a693f82c304c10fc995b44499135bc2ae8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415922"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="42990-104">Obter o status de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="42990-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42990-105">Obter o status de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="42990-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="42990-106">A resposta indicará o status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="42990-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="42990-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="42990-107">Permissions</span></span>
<span data-ttu-id="42990-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42990-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42990-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42990-110">Permission type</span></span> | <span data-ttu-id="42990-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42990-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="42990-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42990-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42990-113">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42990-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="42990-114">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="42990-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="42990-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42990-115">Not supported.</span></span>|
|<span data-ttu-id="42990-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42990-116">Application</span></span>| <span data-ttu-id="42990-117">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="42990-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42990-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42990-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="42990-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42990-119">Request headers</span></span>
| <span data-ttu-id="42990-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42990-120">Name</span></span>       | <span data-ttu-id="42990-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="42990-121">Type</span></span> | <span data-ttu-id="42990-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="42990-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42990-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42990-123">Authorization</span></span>  | <span data-ttu-id="42990-124">string</span><span class="sxs-lookup"><span data-stu-id="42990-124">string</span></span>  | <span data-ttu-id="42990-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42990-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42990-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42990-127">Request body</span></span>
<span data-ttu-id="42990-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42990-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="42990-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42990-129">Response</span></span>
<span data-ttu-id="42990-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42990-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42990-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42990-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42990-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42990-132">Request</span></span>
<span data-ttu-id="42990-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42990-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42990-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="42990-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42990-135">C#</span><span class="sxs-lookup"><span data-stu-id="42990-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42990-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42990-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42990-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="42990-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="42990-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="42990-138">Response</span></span>
<span data-ttu-id="42990-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42990-139">The following is an example of the response.</span></span> 

><span data-ttu-id="42990-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42990-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
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
