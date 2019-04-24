---
title: 'group: unsubscribeByMail'
description: 'Chamar esse método desabilitará o usuário atual para receber notificações por email desse grupo sobre novas postagens, eventos e arquivos nesse grupo. Suportado somente para grupos do Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f7790ad68a99e13454add6db9a9e80229ab21254
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501991"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="cc81f-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="cc81f-104">group: unsubscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc81f-105">Chamar esse método desabilitará o usuário atual para receber notificações por email desse grupo sobre novas postagens, eventos e arquivos nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="cc81f-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="cc81f-106">Suportado somente para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cc81f-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cc81f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc81f-107">Permissions</span></span>
<span data-ttu-id="cc81f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc81f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc81f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc81f-110">Permission type</span></span>      | <span data-ttu-id="cc81f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc81f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc81f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc81f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc81f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc81f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc81f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc81f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc81f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc81f-115">Not supported.</span></span>    |
|<span data-ttu-id="cc81f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc81f-116">Application</span></span> | <span data-ttu-id="cc81f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc81f-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc81f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc81f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="cc81f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc81f-119">Request headers</span></span>
| <span data-ttu-id="cc81f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc81f-120">Header</span></span>       | <span data-ttu-id="cc81f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc81f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc81f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc81f-122">Authorization</span></span>  | <span data-ttu-id="cc81f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc81f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc81f-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="cc81f-125">Prefer</span></span> | <span data-ttu-id="cc81f-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="cc81f-126">return=minimal.</span></span> <span data-ttu-id="cc81f-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cc81f-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="cc81f-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc81f-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="cc81f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc81f-129">Request body</span></span>
 <span data-ttu-id="cc81f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc81f-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="cc81f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc81f-131">Response</span></span>
<span data-ttu-id="cc81f-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc81f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc81f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc81f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc81f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc81f-135">Request</span></span>
<span data-ttu-id="cc81f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc81f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="cc81f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc81f-137">Response</span></span>
<span data-ttu-id="cc81f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc81f-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-unsubscribebymail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
