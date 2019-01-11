---
title: Sincronização de pausa em um educationSynchronizationProfile
description: Pause a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 97ded3f4fdf30e6bc56345abcc71f3466ef4ff61
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892314"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="956dd-103">Sincronização de pausa em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="956dd-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="956dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="956dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="956dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="956dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="956dd-106">Pause a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="956dd-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="956dd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="956dd-107">Permissions</span></span>
<span data-ttu-id="956dd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="956dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="956dd-110">Permission type</span></span> | <span data-ttu-id="956dd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="956dd-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="956dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="956dd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="956dd-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="956dd-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="956dd-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="956dd-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="956dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="956dd-115">Not supported.</span></span>|
|<span data-ttu-id="956dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="956dd-116">Application</span></span>|<span data-ttu-id="956dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="956dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="956dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="956dd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="956dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="956dd-119">Request headers</span></span>
| <span data-ttu-id="956dd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="956dd-120">Name</span></span>       | <span data-ttu-id="956dd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="956dd-121">Type</span></span> | <span data-ttu-id="956dd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="956dd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="956dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="956dd-123">Authorization</span></span>  | <span data-ttu-id="956dd-124">string</span><span class="sxs-lookup"><span data-stu-id="956dd-124">string</span></span>  | <span data-ttu-id="956dd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="956dd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="956dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="956dd-127">Request body</span></span>
<span data-ttu-id="956dd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="956dd-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="956dd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="956dd-129">Response</span></span>
<span data-ttu-id="956dd-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="956dd-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="956dd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="956dd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="956dd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="956dd-132">Request</span></span>
<span data-ttu-id="956dd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="956dd-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="956dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="956dd-134">Response</span></span>

<span data-ttu-id="956dd-135">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="956dd-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
