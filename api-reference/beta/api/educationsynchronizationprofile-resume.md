---
title: Continuar a sincronização em um educationSynchronizationProfile
description: ReTome a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8fd56ec1d825104cb442f9184c1735e34b557fce
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324952"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="1e729-103">Continuar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="1e729-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e729-104">ReTome a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="1e729-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e729-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e729-105">Permissions</span></span>
<span data-ttu-id="1e729-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e729-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e729-108">Permission type</span></span> | <span data-ttu-id="1e729-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e729-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1e729-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e729-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e729-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e729-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1e729-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e729-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1e729-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e729-113">Not supported.</span></span>|
|<span data-ttu-id="1e729-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e729-114">Application</span></span>|<span data-ttu-id="1e729-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e729-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e729-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e729-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="1e729-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e729-117">Request headers</span></span>
| <span data-ttu-id="1e729-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1e729-118">Name</span></span>       | <span data-ttu-id="1e729-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e729-119">Type</span></span> | <span data-ttu-id="1e729-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e729-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1e729-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e729-121">Authorization</span></span>  | <span data-ttu-id="1e729-122">string</span><span class="sxs-lookup"><span data-stu-id="1e729-122">string</span></span>  | <span data-ttu-id="1e729-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e729-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e729-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e729-125">Request body</span></span>
<span data-ttu-id="1e729-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e729-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1e729-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e729-127">Response</span></span>
<span data-ttu-id="1e729-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1e729-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1e729-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e729-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e729-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e729-130">Request</span></span>
<span data-ttu-id="1e729-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e729-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="1e729-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e729-132">Response</span></span>

<span data-ttu-id="1e729-133">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e729-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
