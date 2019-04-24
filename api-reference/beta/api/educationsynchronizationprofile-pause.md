---
title: PaUsar a sincronização em um educationSynchronizationProfile
description: PaUsar a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c9ba7d2ab3f67880105d45d9d98506b8e8caaac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464688"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="f47ca-103">PaUsar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="f47ca-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47ca-104">PaUsar a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="f47ca-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f47ca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f47ca-105">Permissions</span></span>
<span data-ttu-id="f47ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f47ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f47ca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f47ca-108">Permission type</span></span> | <span data-ttu-id="f47ca-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f47ca-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f47ca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f47ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f47ca-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f47ca-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f47ca-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f47ca-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f47ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f47ca-113">Not supported.</span></span>|
|<span data-ttu-id="f47ca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f47ca-114">Application</span></span>|<span data-ttu-id="f47ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f47ca-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f47ca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f47ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="f47ca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f47ca-117">Request headers</span></span>
| <span data-ttu-id="f47ca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f47ca-118">Name</span></span>       | <span data-ttu-id="f47ca-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f47ca-119">Type</span></span> | <span data-ttu-id="f47ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f47ca-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f47ca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f47ca-121">Authorization</span></span>  | <span data-ttu-id="f47ca-122">string</span><span class="sxs-lookup"><span data-stu-id="f47ca-122">string</span></span>  | <span data-ttu-id="f47ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f47ca-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f47ca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f47ca-125">Request body</span></span>
<span data-ttu-id="f47ca-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f47ca-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f47ca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f47ca-127">Response</span></span>
<span data-ttu-id="f47ca-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f47ca-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f47ca-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f47ca-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f47ca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f47ca-130">Request</span></span>
<span data-ttu-id="f47ca-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f47ca-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="f47ca-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f47ca-132">Response</span></span>

<span data-ttu-id="f47ca-133">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f47ca-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
