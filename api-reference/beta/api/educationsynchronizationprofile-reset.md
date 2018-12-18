---
title: Redefinir a sincronização de um educationSynchronizationProfile
description: Redefina a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
ms.openlocfilehash: 29d21318737ceba3bd380eaf20a9500a6a711857
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362437"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="d4450-103">Redefinir a sincronização de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="d4450-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="d4450-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4450-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4450-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4450-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4450-106">Redefina a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="d4450-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="d4450-107">**Observação:** Essa operação fará com que a sincronização reiniciar.</span><span class="sxs-lookup"><span data-stu-id="d4450-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="d4450-108">Quaisquer erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="d4450-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="d4450-109">Nenhum dado será excluído do Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="d4450-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4450-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4450-110">Permissions</span></span>
<span data-ttu-id="d4450-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4450-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4450-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4450-113">Permission type</span></span> | <span data-ttu-id="d4450-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4450-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d4450-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4450-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d4450-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4450-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="d4450-117">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d4450-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d4450-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4450-118">Not supported.</span></span>|
|<span data-ttu-id="d4450-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4450-119">Application</span></span>|<span data-ttu-id="d4450-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4450-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4450-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4450-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="d4450-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4450-122">Request headers</span></span>
| <span data-ttu-id="d4450-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d4450-123">Name</span></span>       | <span data-ttu-id="d4450-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4450-124">Type</span></span> | <span data-ttu-id="d4450-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4450-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4450-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4450-126">Authorization</span></span>  | <span data-ttu-id="d4450-127">string</span><span class="sxs-lookup"><span data-stu-id="d4450-127">string</span></span>  | <span data-ttu-id="d4450-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4450-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4450-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4450-130">Request body</span></span>
<span data-ttu-id="d4450-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4450-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d4450-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4450-132">Response</span></span>
<span data-ttu-id="d4450-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d4450-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d4450-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4450-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4450-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4450-135">Request</span></span>
<span data-ttu-id="d4450-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4450-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="d4450-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4450-137">Response</span></span>

<span data-ttu-id="d4450-138">Não há nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4450-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```