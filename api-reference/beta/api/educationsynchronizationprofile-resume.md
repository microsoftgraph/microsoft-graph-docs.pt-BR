---
title: Reiniciar a sincronização de um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escola específico no inquilino.
ms.openlocfilehash: a184c6d7903da891d93275f87501ab38f83c3e88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038080"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e4cae-103">Reiniciar a sincronização de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e4cae-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="e4cae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4cae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4cae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4cae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4cae-106">Retome a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="e4cae-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4cae-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e4cae-107">Permissions</span></span>
<span data-ttu-id="e4cae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4cae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4cae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4cae-110">Permission type</span></span> | <span data-ttu-id="e4cae-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e4cae-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e4cae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4cae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4cae-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4cae-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e4cae-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e4cae-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e4cae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4cae-115">Not supported.</span></span>|
|<span data-ttu-id="e4cae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4cae-116">Application</span></span>|<span data-ttu-id="e4cae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4cae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4cae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4cae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="e4cae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4cae-119">Request headers</span></span>
| <span data-ttu-id="e4cae-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e4cae-120">Name</span></span>       | <span data-ttu-id="e4cae-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4cae-121">Type</span></span> | <span data-ttu-id="e4cae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4cae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4cae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4cae-123">Authorization</span></span>  | <span data-ttu-id="e4cae-124">string</span><span class="sxs-lookup"><span data-stu-id="e4cae-124">string</span></span>  | <span data-ttu-id="e4cae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4cae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4cae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4cae-127">Request body</span></span>
<span data-ttu-id="e4cae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4cae-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e4cae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4cae-129">Response</span></span>
<span data-ttu-id="e4cae-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e4cae-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4cae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4cae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4cae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4cae-132">Request</span></span>
<span data-ttu-id="e4cae-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4cae-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="e4cae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4cae-134">Response</span></span>

<span data-ttu-id="e4cae-135">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4cae-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```