---
title: Excluir bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 273c3f3578653e457122b2bf045eb54644ea6b08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849914"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="78393-104">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="78393-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="78393-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78393-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78393-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78393-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="78393-107">Exclua um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="78393-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="78393-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="78393-108">Permissions</span></span>
<span data-ttu-id="78393-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78393-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78393-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78393-111">Permission type</span></span>      | <span data-ttu-id="78393-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78393-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78393-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78393-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="78393-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="78393-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="78393-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78393-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78393-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78393-116">Not supported.</span></span>   |
|<span data-ttu-id="78393-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78393-117">Application</span></span> | <span data-ttu-id="78393-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78393-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="78393-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78393-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="78393-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78393-120">Request headers</span></span>
| <span data-ttu-id="78393-121">Nome</span><span class="sxs-lookup"><span data-stu-id="78393-121">Name</span></span>       | <span data-ttu-id="78393-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="78393-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78393-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78393-123">Authorization</span></span>  | <span data-ttu-id="78393-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="78393-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="78393-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78393-125">Request body</span></span>
<span data-ttu-id="78393-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78393-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="78393-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="78393-127">Response</span></span>
<span data-ttu-id="78393-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78393-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78393-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78393-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78393-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78393-131">Request</span></span>
<span data-ttu-id="78393-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78393-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="78393-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78393-133">Response</span></span>
<span data-ttu-id="78393-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78393-134">The following is an example of the response.</span></span> 
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
