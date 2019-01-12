---
title: Excluir bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7616e04c25aefedde084fc47c06d22410f9f0fee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991220"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="a1a73-104">Excluir bookingService</span><span class="sxs-lookup"><span data-stu-id="a1a73-104">Delete bookingService</span></span>

 > <span data-ttu-id="a1a73-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1a73-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1a73-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1a73-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a1a73-107">Exclua um objeto [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a1a73-107">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a1a73-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1a73-108">Permissions</span></span>
<span data-ttu-id="a1a73-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1a73-111">Permission type</span></span>      | <span data-ttu-id="a1a73-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1a73-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1a73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1a73-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1a73-114">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a1a73-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a1a73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1a73-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1a73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a73-116">Not supported.</span></span>   |
|<span data-ttu-id="a1a73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1a73-117">Application</span></span> | <span data-ttu-id="a1a73-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a73-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a1a73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1a73-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a1a73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a73-120">Request headers</span></span>
| <span data-ttu-id="a1a73-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a1a73-121">Name</span></span>       | <span data-ttu-id="a1a73-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1a73-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1a73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1a73-123">Authorization</span></span>  | <span data-ttu-id="a1a73-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a1a73-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a73-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a73-125">Request body</span></span>
<span data-ttu-id="a1a73-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1a73-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a1a73-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a73-127">Response</span></span>
<span data-ttu-id="a1a73-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1a73-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a73-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1a73-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1a73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a73-131">Request</span></span>
<span data-ttu-id="a1a73-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1a73-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="a1a73-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a73-133">Response</span></span>
<span data-ttu-id="a1a73-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1a73-134">The following is an example of the response.</span></span> <span data-ttu-id="a1a73-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a1a73-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a1a73-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1a73-136">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
