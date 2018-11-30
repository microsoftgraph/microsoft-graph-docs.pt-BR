---
title: Excluir um educationSynchronizationProfile
description: Exclua um perfil de sincronização de dados escola no locatário com base no identificador.
ms.openlocfilehash: 829b723b48eb9a15750bc9d0e00ba50d432e8ab6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037772"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="d1c2a-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="d1c2a-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="d1c2a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1c2a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1c2a-106">Exclua um de dados da escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1c2a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1c2a-107">Permissions</span></span>
<span data-ttu-id="d1c2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1c2a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1c2a-110">Permission type</span></span> | <span data-ttu-id="d1c2a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1c2a-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d1c2a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1c2a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1c2a-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1c2a-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1c2a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1c2a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1c2a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c2a-115">Request headers</span></span>
| <span data-ttu-id="d1c2a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d1c2a-116">Name</span></span>       | <span data-ttu-id="d1c2a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1c2a-117">Type</span></span> | <span data-ttu-id="d1c2a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1c2a-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1c2a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1c2a-119">Authorization</span></span>  | <span data-ttu-id="d1c2a-120">string</span><span class="sxs-lookup"><span data-stu-id="d1c2a-120">string</span></span>  | <span data-ttu-id="d1c2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="d1c2a-123">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d1c2a-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d1c2a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-124">Not supported.</span></span>|
|<span data-ttu-id="d1c2a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1c2a-125">Application</span></span>|<span data-ttu-id="d1c2a-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c2a-127">Request body</span></span>
<span data-ttu-id="d1c2a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1c2a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c2a-129">Response</span></span>
<span data-ttu-id="d1c2a-130">Se bem-sucedido, este método retorna o código de resposta `202 Accepted` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c2a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1c2a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1c2a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c2a-132">Request</span></span>
<span data-ttu-id="d1c2a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="d1c2a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c2a-134">Response</span></span>
<span data-ttu-id="d1c2a-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c2a-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
