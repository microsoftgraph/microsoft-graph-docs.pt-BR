---
title: Excluir bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 16ee4c5fa244e3507238abd0a696b31477173e11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819772"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="fc318-104">Excluir bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="fc318-104">Delete bookingStaffMember</span></span>

 > <span data-ttu-id="fc318-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc318-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc318-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc318-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="fc318-107">Exclua um [membro da equipe](../resources/bookingstaffmember.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="fc318-107">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fc318-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="fc318-108">Permissions</span></span>
<span data-ttu-id="fc318-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc318-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc318-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc318-111">Permission type</span></span>      | <span data-ttu-id="fc318-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc318-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc318-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc318-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc318-114">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fc318-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fc318-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc318-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc318-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc318-116">Not supported.</span></span>   |
|<span data-ttu-id="fc318-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc318-117">Application</span></span> | <span data-ttu-id="fc318-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc318-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fc318-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc318-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fc318-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc318-120">Request headers</span></span>
| <span data-ttu-id="fc318-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fc318-121">Name</span></span>       | <span data-ttu-id="fc318-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc318-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc318-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc318-123">Authorization</span></span>  | <span data-ttu-id="fc318-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fc318-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc318-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc318-125">Request body</span></span>
<span data-ttu-id="fc318-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc318-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fc318-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc318-127">Response</span></span>
<span data-ttu-id="fc318-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc318-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc318-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc318-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc318-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc318-131">Request</span></span>
<span data-ttu-id="fc318-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc318-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="fc318-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc318-133">Response</span></span>
<span data-ttu-id="fc318-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc318-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
