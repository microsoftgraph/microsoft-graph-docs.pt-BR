---
title: Excluir um educationSynchronizationProfile
description: Excluir um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457449"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="de0d6-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="de0d6-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de0d6-104">Excluir um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="de0d6-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="de0d6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de0d6-105">Permissions</span></span>
<span data-ttu-id="de0d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de0d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de0d6-108">Permission type</span></span> | <span data-ttu-id="de0d6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="de0d6-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="de0d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de0d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de0d6-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de0d6-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="de0d6-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de0d6-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="de0d6-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de0d6-113">Request headers</span></span>
| <span data-ttu-id="de0d6-114">Nome</span><span class="sxs-lookup"><span data-stu-id="de0d6-114">Name</span></span>       | <span data-ttu-id="de0d6-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="de0d6-115">Type</span></span> | <span data-ttu-id="de0d6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="de0d6-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de0d6-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="de0d6-117">Authorization</span></span>  | <span data-ttu-id="de0d6-118">string</span><span class="sxs-lookup"><span data-stu-id="de0d6-118">string</span></span>  | <span data-ttu-id="de0d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de0d6-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="de0d6-121">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="de0d6-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="de0d6-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de0d6-122">Not supported.</span></span>|
|<span data-ttu-id="de0d6-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de0d6-123">Application</span></span>|<span data-ttu-id="de0d6-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de0d6-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de0d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de0d6-125">Request body</span></span>
<span data-ttu-id="de0d6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de0d6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de0d6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0d6-127">Response</span></span>
<span data-ttu-id="de0d6-128">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de0d6-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="de0d6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de0d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de0d6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de0d6-130">Request</span></span>
<span data-ttu-id="de0d6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de0d6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="de0d6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0d6-132">Response</span></span>
<span data-ttu-id="de0d6-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de0d6-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
