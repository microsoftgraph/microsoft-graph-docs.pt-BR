---
title: Excluir um educationSynchronizationProfile
description: Exclua um perfil de sincronização de dados escola no locatário com base no identificador.
author: mmast-msft
ms.openlocfilehash: b0287133d579915279e0f9a02bf49dd981ccf419
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343299"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="73a9c-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="73a9c-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="73a9c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73a9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73a9c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73a9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73a9c-106">Exclua um de dados da escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="73a9c-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a9c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="73a9c-107">Permissions</span></span>
<span data-ttu-id="73a9c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73a9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73a9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73a9c-110">Permission type</span></span> | <span data-ttu-id="73a9c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="73a9c-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="73a9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73a9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73a9c-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73a9c-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73a9c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73a9c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73a9c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73a9c-115">Request headers</span></span>
| <span data-ttu-id="73a9c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="73a9c-116">Name</span></span>       | <span data-ttu-id="73a9c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="73a9c-117">Type</span></span> | <span data-ttu-id="73a9c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a9c-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73a9c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="73a9c-119">Authorization</span></span>  | <span data-ttu-id="73a9c-120">string</span><span class="sxs-lookup"><span data-stu-id="73a9c-120">string</span></span>  | <span data-ttu-id="73a9c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73a9c-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="73a9c-123">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="73a9c-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="73a9c-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73a9c-124">Not supported.</span></span>|
|<span data-ttu-id="73a9c-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73a9c-125">Application</span></span>|<span data-ttu-id="73a9c-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73a9c-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73a9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73a9c-127">Request body</span></span>
<span data-ttu-id="73a9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73a9c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73a9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="73a9c-129">Response</span></span>
<span data-ttu-id="73a9c-130">Se bem-sucedido, este método retorna o código de resposta `202 Accepted` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73a9c-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="73a9c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73a9c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73a9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73a9c-132">Request</span></span>
<span data-ttu-id="73a9c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73a9c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="73a9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73a9c-134">Response</span></span>
<span data-ttu-id="73a9c-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73a9c-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
