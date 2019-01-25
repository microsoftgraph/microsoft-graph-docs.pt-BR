---
title: Reiniciar a sincronização de um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 50ffcb4ceab401a3041ecb69baa1de0409be94a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513253"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="20ca4-103">Reiniciar a sincronização de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="20ca4-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ca4-104">Retome a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="20ca4-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="20ca4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="20ca4-105">Permissions</span></span>
<span data-ttu-id="20ca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20ca4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20ca4-108">Permission type</span></span> | <span data-ttu-id="20ca4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="20ca4-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="20ca4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20ca4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20ca4-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20ca4-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="20ca4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20ca4-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="20ca4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20ca4-113">Not supported.</span></span>|
|<span data-ttu-id="20ca4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20ca4-114">Application</span></span>|<span data-ttu-id="20ca4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20ca4-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20ca4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20ca4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="20ca4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20ca4-117">Request headers</span></span>
| <span data-ttu-id="20ca4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="20ca4-118">Name</span></span>       | <span data-ttu-id="20ca4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ca4-119">Type</span></span> | <span data-ttu-id="20ca4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ca4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20ca4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20ca4-121">Authorization</span></span>  | <span data-ttu-id="20ca4-122">string</span><span class="sxs-lookup"><span data-stu-id="20ca4-122">string</span></span>  | <span data-ttu-id="20ca4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ca4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="20ca4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20ca4-125">Request body</span></span>
<span data-ttu-id="20ca4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20ca4-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="20ca4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ca4-127">Response</span></span>
<span data-ttu-id="20ca4-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="20ca4-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20ca4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20ca4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20ca4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20ca4-130">Request</span></span>
<span data-ttu-id="20ca4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ca4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="20ca4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ca4-132">Response</span></span>

<span data-ttu-id="20ca4-133">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20ca4-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
