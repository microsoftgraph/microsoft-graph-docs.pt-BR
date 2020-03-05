---
title: Obter o status de um educationSynchronizationProfile
description: Obter o status de um perfil de sincronização de dados escolar específico no locatário. A resposta indicará o status da sincronização.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b9683a7f97ca2610efd8fd91a762dffd26a3e3b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424103"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="3dba0-104">Obter o status de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="3dba0-104">Get the status of an educationSynchronizationProfile</span></span>

<span data-ttu-id="3dba0-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3dba0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dba0-106">Obter o status de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="3dba0-106">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="3dba0-107">A resposta indicará o status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="3dba0-107">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dba0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dba0-108">Permissions</span></span>
<span data-ttu-id="3dba0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dba0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dba0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dba0-111">Permission type</span></span> | <span data-ttu-id="3dba0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dba0-112">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3dba0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dba0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3dba0-114">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3dba0-114">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3dba0-115">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3dba0-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3dba0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dba0-116">Not supported.</span></span>|
|<span data-ttu-id="3dba0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dba0-117">Application</span></span>| <span data-ttu-id="3dba0-118">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3dba0-118">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dba0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dba0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="3dba0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dba0-120">Request headers</span></span>
| <span data-ttu-id="3dba0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3dba0-121">Name</span></span>       | <span data-ttu-id="3dba0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dba0-122">Type</span></span> | <span data-ttu-id="3dba0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dba0-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3dba0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dba0-124">Authorization</span></span>  | <span data-ttu-id="3dba0-125">string</span><span class="sxs-lookup"><span data-stu-id="3dba0-125">string</span></span>  | <span data-ttu-id="3dba0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dba0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3dba0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dba0-128">Request body</span></span>
<span data-ttu-id="3dba0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dba0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3dba0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dba0-130">Response</span></span>
<span data-ttu-id="3dba0-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dba0-131">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dba0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dba0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3dba0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dba0-133">Request</span></span>
<span data-ttu-id="3dba0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dba0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dba0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dba0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[<span data-ttu-id="3dba0-136">C#</span><span class="sxs-lookup"><span data-stu-id="3dba0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dba0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dba0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dba0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dba0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3dba0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dba0-139">Response</span></span>
<span data-ttu-id="3dba0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3dba0-140">The following is an example of the response.</span></span> 

><span data-ttu-id="3dba0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dba0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
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
