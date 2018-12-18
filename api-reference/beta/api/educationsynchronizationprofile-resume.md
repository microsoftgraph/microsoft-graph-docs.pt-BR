---
title: Reiniciar a sincronização de um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
ms.openlocfilehash: fd148db59d34f6455ba01e721453972f9cf65be4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305646"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="056cd-103">Reiniciar a sincronização de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="056cd-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="056cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="056cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="056cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="056cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="056cd-106">Retome a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="056cd-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="056cd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="056cd-107">Permissions</span></span>
<span data-ttu-id="056cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="056cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="056cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="056cd-110">Permission type</span></span> | <span data-ttu-id="056cd-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="056cd-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="056cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="056cd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="056cd-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="056cd-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="056cd-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="056cd-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="056cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="056cd-115">Not supported.</span></span>|
|<span data-ttu-id="056cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="056cd-116">Application</span></span>|<span data-ttu-id="056cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="056cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="056cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="056cd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="056cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="056cd-119">Request headers</span></span>
| <span data-ttu-id="056cd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="056cd-120">Name</span></span>       | <span data-ttu-id="056cd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="056cd-121">Type</span></span> | <span data-ttu-id="056cd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="056cd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="056cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="056cd-123">Authorization</span></span>  | <span data-ttu-id="056cd-124">string</span><span class="sxs-lookup"><span data-stu-id="056cd-124">string</span></span>  | <span data-ttu-id="056cd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="056cd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="056cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="056cd-127">Request body</span></span>
<span data-ttu-id="056cd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="056cd-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="056cd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="056cd-129">Response</span></span>
<span data-ttu-id="056cd-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="056cd-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="056cd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="056cd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="056cd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="056cd-132">Request</span></span>
<span data-ttu-id="056cd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="056cd-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="056cd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="056cd-134">Response</span></span>

<span data-ttu-id="056cd-135">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="056cd-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```