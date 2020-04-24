---
title: Criar um permitido
description: Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ce8080503f45a79dae422186ab360bc0e4071dd0
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807061"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="5f36c-103">Criar um permitido</span><span class="sxs-lookup"><span data-stu-id="5f36c-103">Create allowedGroup</span></span>

<span data-ttu-id="5f36c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f36c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f36c-105">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="5f36c-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f36c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f36c-106">Permissions</span></span>
<span data-ttu-id="5f36c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f36c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5f36c-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="5f36c-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5f36c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f36c-110">Permission type</span></span> | <span data-ttu-id="5f36c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f36c-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5f36c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f36c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5f36c-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f36c-113">Users.Read.All</span></span> |
|<span data-ttu-id="5f36c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f36c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f36c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f36c-115">Not Supported.</span></span>|
|<span data-ttu-id="5f36c-116">Application</span><span class="sxs-lookup"><span data-stu-id="5f36c-116">Application</span></span>|<span data-ttu-id="5f36c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f36c-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f36c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f36c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5f36c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f36c-119">Request headers</span></span>
| <span data-ttu-id="5f36c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5f36c-120">Name</span></span>          | <span data-ttu-id="5f36c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f36c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5f36c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f36c-122">Authorization</span></span> | <span data-ttu-id="5f36c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f36c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f36c-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="5f36c-125">Content-type</span></span>  | <span data-ttu-id="5f36c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f36c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f36c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f36c-128">Request body</span></span>
<span data-ttu-id="5f36c-129">No corpo da solicitação, forneça uma referência a uma entidade de grupo usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f36c-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="5f36c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f36c-130">Response</span></span>
<span data-ttu-id="5f36c-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="5f36c-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f36c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f36c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f36c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f36c-133">Request</span></span>
<span data-ttu-id="5f36c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f36c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```

<span data-ttu-id="5f36c-135">No corpo da solicitação, forneça uma referência a uma entidade de grupo incluindo o URI do Microsoft Graph do grupo no `@odata.id` campo do corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="5f36c-135">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="5f36c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f36c-136">Response</span></span>
<span data-ttu-id="5f36c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f36c-137">The following is an example of the response.</span></span> 
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
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
