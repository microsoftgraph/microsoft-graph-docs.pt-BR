---
title: Criar allowedUser
description: Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8f4e7ce70d8374d1c04cb6d69feaf33b69b5e954
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807059"
---
# <a name="create-alloweduser"></a><span data-ttu-id="0f066-103">Criar allowedUser</span><span class="sxs-lookup"><span data-stu-id="0f066-103">Create allowedUser</span></span>

<span data-ttu-id="0f066-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f066-105">Conceda ao usuário especificado acesso para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="0f066-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f066-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f066-106">Permissions</span></span>
<span data-ttu-id="0f066-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0f066-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="0f066-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0f066-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f066-110">Permission type</span></span> | <span data-ttu-id="0f066-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f066-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0f066-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f066-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0f066-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="0f066-113">Users.Read.All</span></span> |
|<span data-ttu-id="0f066-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f066-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f066-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f066-115">Not Supported.</span></span>|
|<span data-ttu-id="0f066-116">Application</span><span class="sxs-lookup"><span data-stu-id="0f066-116">Application</span></span>|<span data-ttu-id="0f066-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f066-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f066-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f066-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0f066-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f066-119">Request headers</span></span>
| <span data-ttu-id="0f066-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0f066-120">Name</span></span>          | <span data-ttu-id="0f066-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f066-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f066-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f066-122">Authorization</span></span> | <span data-ttu-id="0f066-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f066-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f066-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0f066-125">Content-type</span></span>  | <span data-ttu-id="0f066-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f066-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f066-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f066-128">Request body</span></span>
<span data-ttu-id="0f066-129">No corpo da solicitação, forneça uma referência a uma entidade de usuário usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="0f066-129">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="0f066-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f066-130">Response</span></span>
<span data-ttu-id="0f066-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="0f066-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f066-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f066-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f066-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f066-133">Request</span></span>
<span data-ttu-id="0f066-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f066-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_alloweduser_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares/{id}/allowedUsers/$ref
Content-type: application/json
Content-length: 66

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
<span data-ttu-id="0f066-135">No corpo da solicitação, forneça uma referência a uma entidade de usuário, incluindo o URI do Microsoft Graph do usuário `@odata.id` no campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="0f066-135">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="0f066-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f066-136">Response</span></span>
<span data-ttu-id="0f066-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f066-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
