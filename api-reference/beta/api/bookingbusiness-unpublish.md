---
title: 'bookingBusiness: cancelamento de publicação'
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 7d0e083eded3ce0c1328c9532358cf7a054db52b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035334"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="46e46-104">bookingBusiness: cancelamento de publicação</span><span class="sxs-lookup"><span data-stu-id="46e46-104">bookingBusiness: unpublish</span></span>

 > <span data-ttu-id="46e46-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46e46-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46e46-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46e46-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="46e46-107">Verifique a página de agendamento dessa empresa não está disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="46e46-107">Make the scheduling page of this business not available to external customers.</span></span> 

<span data-ttu-id="46e46-108">Defina a propriedade **isPublished** como false e a propriedade **publicUrl** como nulo.</span><span class="sxs-lookup"><span data-stu-id="46e46-108">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="46e46-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="46e46-109">Permissions</span></span>
<span data-ttu-id="46e46-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e46-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46e46-112">Permission type</span></span>      | <span data-ttu-id="46e46-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46e46-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46e46-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46e46-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="46e46-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="46e46-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="46e46-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46e46-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46e46-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e46-117">Not supported.</span></span>   |
|<span data-ttu-id="46e46-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46e46-118">Application</span></span> | <span data-ttu-id="46e46-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e46-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="46e46-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46e46-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="46e46-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46e46-121">Request headers</span></span>
| <span data-ttu-id="46e46-122">Nome</span><span class="sxs-lookup"><span data-stu-id="46e46-122">Name</span></span>       | <span data-ttu-id="46e46-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e46-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46e46-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46e46-124">Authorization</span></span>  | <span data-ttu-id="46e46-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="46e46-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e46-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46e46-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="46e46-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e46-127">Response</span></span>
<span data-ttu-id="46e46-p104">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46e46-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e46-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46e46-130">Example</span></span>
<span data-ttu-id="46e46-131">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="46e46-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46e46-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46e46-132">Request</span></span>
<span data-ttu-id="46e46-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46e46-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="46e46-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e46-134">Response</span></span>
<span data-ttu-id="46e46-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46e46-135">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->