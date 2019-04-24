---
title: Redefinir a sincronização em um educationSynchronizationProfile
description: Redefinir a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457500"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="3cd71-103">Redefinir a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="3cd71-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd71-104">Redefinir a sincronização de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="3cd71-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="3cd71-105">**Observação:** Essa operação causará a reinicialização da sincronização.</span><span class="sxs-lookup"><span data-stu-id="3cd71-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="3cd71-106">Os erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="3cd71-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="3cd71-107">Nenhum dado será excluído do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3cd71-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="3cd71-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd71-108">Permissions</span></span>
<span data-ttu-id="3cd71-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cd71-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd71-111">Permission type</span></span> | <span data-ttu-id="3cd71-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd71-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3cd71-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd71-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3cd71-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cd71-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3cd71-115">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3cd71-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3cd71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd71-116">Not supported.</span></span>|
|<span data-ttu-id="3cd71-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd71-117">Application</span></span>|<span data-ttu-id="3cd71-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd71-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="3cd71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd71-120">Request headers</span></span>
| <span data-ttu-id="3cd71-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3cd71-121">Name</span></span>       | <span data-ttu-id="3cd71-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd71-122">Type</span></span> | <span data-ttu-id="3cd71-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd71-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3cd71-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd71-124">Authorization</span></span>  | <span data-ttu-id="3cd71-125">string</span><span class="sxs-lookup"><span data-stu-id="3cd71-125">string</span></span>  | <span data-ttu-id="3cd71-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd71-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cd71-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd71-128">Request body</span></span>
<span data-ttu-id="3cd71-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cd71-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3cd71-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd71-130">Response</span></span>
<span data-ttu-id="3cd71-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3cd71-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3cd71-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cd71-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cd71-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd71-133">Request</span></span>
<span data-ttu-id="3cd71-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd71-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="3cd71-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd71-135">Response</span></span>

<span data-ttu-id="3cd71-136">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd71-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
