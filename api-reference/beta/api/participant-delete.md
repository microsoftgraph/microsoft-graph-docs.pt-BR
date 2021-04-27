---
title: Excluir participante
description: Exclua um participante específico em uma chamada.
manager: zhengni
author: jackry6350
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1ee50cd399b974b80fcb80ad514bbf3423c0471e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037869"
---
# <a name="delete-participant"></a><span data-ttu-id="e323b-103">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="e323b-103">Delete participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e323b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e323b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e323b-105">Exclua um participante específico em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="e323b-105">Delete a specific participant in a call.</span></span> <span data-ttu-id="e323b-106">Em algumas situações, é apropriado que um aplicativo remova um participante de uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="e323b-106">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="e323b-107">Essa ação pode ser feita depois que o participante responder à chamada.</span><span class="sxs-lookup"><span data-stu-id="e323b-107">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="e323b-108">Quando um chamador ativo é removido, ele é imediatamente removido da chamada sem notificação de pré ou pós-remoção.</span><span class="sxs-lookup"><span data-stu-id="e323b-108">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="e323b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e323b-109">Permissions</span></span>
<span data-ttu-id="e323b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e323b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e323b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e323b-112">Permission type</span></span>                        | <span data-ttu-id="e323b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e323b-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e323b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e323b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e323b-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e323b-115">Not Supported</span></span>                               |
| <span data-ttu-id="e323b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e323b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e323b-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e323b-117">Not Supported</span></span>                               |
| <span data-ttu-id="e323b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e323b-118">Application</span></span>                            | <span data-ttu-id="e323b-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e323b-119">None</span></span>                                        |

<span data-ttu-id="e323b-120">A configuração de reunião de aplicativo no nível de locatário é necessária para permitir que um aplicativo chame essa API.</span><span class="sxs-lookup"><span data-stu-id="e323b-120">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="e323b-121">O administrador do locatário deve chamar o cmdlet a seguir no PowerShell remoto do locatário para conceder a permissão ao aplicativo para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e323b-121">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="e323b-122">Para obter mais informações, [consulte Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e323b-122">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="e323b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e323b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="e323b-124">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e323b-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e323b-125">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e323b-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e323b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e323b-126">Request headers</span></span>
| <span data-ttu-id="e323b-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e323b-127">Name</span></span>          | <span data-ttu-id="e323b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e323b-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e323b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e323b-129">Authorization</span></span> | <span data-ttu-id="e323b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e323b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e323b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e323b-132">Request body</span></span>
<span data-ttu-id="e323b-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e323b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e323b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e323b-134">Response</span></span>
<span data-ttu-id="e323b-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e323b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e323b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e323b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e323b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e323b-138">Request</span></span>
<span data-ttu-id="e323b-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e323b-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e323b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e323b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="e323b-141">C#</span><span class="sxs-lookup"><span data-stu-id="e323b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e323b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e323b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e323b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e323b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e323b-144">Java</span><span class="sxs-lookup"><span data-stu-id="e323b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e323b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e323b-145">Response</span></span>

> <span data-ttu-id="e323b-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e323b-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
