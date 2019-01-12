---
title: Sincronização de pausa em um educationSynchronizationProfile
description: Pause a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950680"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="5a98b-103">Sincronização de pausa em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="5a98b-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="5a98b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a98b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a98b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a98b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a98b-106">Pause a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="5a98b-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a98b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a98b-107">Permissions</span></span>
<span data-ttu-id="5a98b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a98b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a98b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a98b-110">Permission type</span></span> | <span data-ttu-id="5a98b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a98b-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5a98b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a98b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a98b-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a98b-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5a98b-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="5a98b-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5a98b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a98b-115">Not supported.</span></span>|
|<span data-ttu-id="5a98b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a98b-116">Application</span></span>|<span data-ttu-id="5a98b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a98b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a98b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a98b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="5a98b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a98b-119">Request headers</span></span>
| <span data-ttu-id="5a98b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5a98b-120">Name</span></span>       | <span data-ttu-id="5a98b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a98b-121">Type</span></span> | <span data-ttu-id="5a98b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a98b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5a98b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a98b-123">Authorization</span></span>  | <span data-ttu-id="5a98b-124">string</span><span class="sxs-lookup"><span data-stu-id="5a98b-124">string</span></span>  | <span data-ttu-id="5a98b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a98b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a98b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a98b-127">Request body</span></span>
<span data-ttu-id="5a98b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a98b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a98b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a98b-129">Response</span></span>
<span data-ttu-id="5a98b-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5a98b-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5a98b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a98b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a98b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a98b-132">Request</span></span>
<span data-ttu-id="5a98b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a98b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="5a98b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a98b-134">Response</span></span>

<span data-ttu-id="5a98b-135">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a98b-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
