---
title: Excluir bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: c4ba9267e2a3fde3ac43460160ffd4bb37cfb56d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035019"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="e1105-104">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="e1105-104">Delete bookingCustomer</span></span>

 > <span data-ttu-id="e1105-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1105-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1105-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1105-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e1105-107">Exclua o objeto especificado [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="e1105-107">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1105-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1105-108">Permissions</span></span>
<span data-ttu-id="e1105-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1105-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1105-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1105-111">Permission type</span></span>      | <span data-ttu-id="e1105-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1105-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1105-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1105-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1105-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e1105-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e1105-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1105-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1105-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1105-116">Not supported.</span></span>   |
|<span data-ttu-id="e1105-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1105-117">Application</span></span> | <span data-ttu-id="e1105-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1105-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e1105-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1105-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e1105-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1105-120">Request headers</span></span>
| <span data-ttu-id="e1105-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e1105-121">Name</span></span>       | <span data-ttu-id="e1105-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1105-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1105-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1105-123">Authorization</span></span>  | <span data-ttu-id="e1105-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e1105-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1105-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1105-125">Request body</span></span>
<span data-ttu-id="e1105-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1105-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e1105-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1105-127">Response</span></span>
<span data-ttu-id="e1105-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1105-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1105-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1105-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1105-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1105-131">Request</span></span>
<span data-ttu-id="e1105-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1105-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="e1105-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1105-133">Response</span></span>
<span data-ttu-id="e1105-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1105-134">The following is an example of the response.</span></span> <span data-ttu-id="e1105-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e1105-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1105-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1105-136">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->