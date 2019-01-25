---
title: Obter o status de um educationSynchronizationProfile
description: Obter o status de um perfil de sincronização de dados específicos escola no inquilino. A resposta indicará que o status da sincronização.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510194"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="bb902-104">Obter o status de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="bb902-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb902-105">Obter o status de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="bb902-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="bb902-106">A resposta indicará que o status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="bb902-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb902-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb902-107">Permissions</span></span>
<span data-ttu-id="bb902-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb902-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb902-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb902-110">Permission type</span></span> | <span data-ttu-id="bb902-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb902-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bb902-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb902-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb902-113">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb902-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="bb902-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb902-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bb902-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb902-115">Not supported.</span></span>|
|<span data-ttu-id="bb902-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb902-116">Application</span></span>| <span data-ttu-id="bb902-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb902-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb902-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb902-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="bb902-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb902-119">Request headers</span></span>
| <span data-ttu-id="bb902-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bb902-120">Name</span></span>       | <span data-ttu-id="bb902-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb902-121">Type</span></span> | <span data-ttu-id="bb902-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb902-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb902-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb902-123">Authorization</span></span>  | <span data-ttu-id="bb902-124">string</span><span class="sxs-lookup"><span data-stu-id="bb902-124">string</span></span>  | <span data-ttu-id="bb902-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb902-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb902-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb902-127">Request body</span></span>
<span data-ttu-id="bb902-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb902-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bb902-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb902-129">Response</span></span>
<span data-ttu-id="bb902-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb902-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb902-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb902-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb902-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb902-132">Request</span></span>
<span data-ttu-id="bb902-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb902-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="bb902-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb902-134">Response</span></span>
<span data-ttu-id="bb902-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb902-135">The following is an example of the response.</span></span> 

><span data-ttu-id="bb902-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb902-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
