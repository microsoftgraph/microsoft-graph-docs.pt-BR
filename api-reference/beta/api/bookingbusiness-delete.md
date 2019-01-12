---
title: Excluir bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d713d6320e9a221405bd3ab9335bd90204e651a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922393"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="1523c-104">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="1523c-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="1523c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1523c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1523c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1523c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1523c-107">Exclua um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="1523c-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1523c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1523c-108">Permissions</span></span>
<span data-ttu-id="1523c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1523c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1523c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1523c-111">Permission type</span></span>      | <span data-ttu-id="1523c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1523c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1523c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1523c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1523c-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1523c-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1523c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1523c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1523c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1523c-116">Not supported.</span></span>   |
|<span data-ttu-id="1523c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1523c-117">Application</span></span> | <span data-ttu-id="1523c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1523c-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1523c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1523c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="1523c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1523c-120">Request headers</span></span>
| <span data-ttu-id="1523c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1523c-121">Name</span></span>       | <span data-ttu-id="1523c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1523c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1523c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1523c-123">Authorization</span></span>  | <span data-ttu-id="1523c-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1523c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1523c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1523c-125">Request body</span></span>
<span data-ttu-id="1523c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1523c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1523c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1523c-127">Response</span></span>
<span data-ttu-id="1523c-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1523c-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1523c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1523c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1523c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1523c-131">Request</span></span>
<span data-ttu-id="1523c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1523c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="1523c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1523c-133">Response</span></span>
<span data-ttu-id="1523c-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1523c-134">The following is an example of the response.</span></span> 
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
