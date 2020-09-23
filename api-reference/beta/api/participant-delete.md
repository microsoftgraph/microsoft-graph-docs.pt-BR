---
title: Excluir participante
description: Excluir um participante específico em uma chamada.
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 912cb7ce6c4656fa47cbf49c1e78a57f5fcd4f11
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222890"
---
# <a name="delete-participant"></a><span data-ttu-id="85698-103">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="85698-103">Delete participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85698-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85698-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85698-105">Excluir um participante específico em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="85698-105">Delete a specific participant in a call.</span></span> <span data-ttu-id="85698-106">Em algumas situações, é apropriado que um aplicativo remova um participante de uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="85698-106">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="85698-107">Esta ação pode ser feita após o participante responder a chamada.</span><span class="sxs-lookup"><span data-stu-id="85698-107">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="85698-108">Quando um chamador ativo é removido, ele é imediatamente descartado da chamada sem notificação prévia ou após a remoção.</span><span class="sxs-lookup"><span data-stu-id="85698-108">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="85698-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="85698-109">Permissions</span></span>
<span data-ttu-id="85698-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85698-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85698-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85698-112">Permission type</span></span>                        | <span data-ttu-id="85698-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85698-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85698-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85698-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="85698-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="85698-115">Not Supported</span></span>                               |
| <span data-ttu-id="85698-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85698-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85698-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="85698-117">Not Supported</span></span>                               |
| <span data-ttu-id="85698-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85698-118">Application</span></span>                            | <span data-ttu-id="85698-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85698-119">None</span></span>                                        |

<span data-ttu-id="85698-120">A configuração de reunião de aplicativo em nível de locatário é necessária para permitir que um aplicativo chame esta API.</span><span class="sxs-lookup"><span data-stu-id="85698-120">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="85698-121">O administrador do locatário deve chamar o seguinte cmdlet no PowerShell remoto do locatário para conceder a permissão ao aplicativo para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="85698-121">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="85698-122">Para obter mais informações, consulte [set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85698-122">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="85698-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85698-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="85698-124">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="85698-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="85698-125">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="85698-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85698-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85698-126">Request headers</span></span>
| <span data-ttu-id="85698-127">Nome</span><span class="sxs-lookup"><span data-stu-id="85698-127">Name</span></span>          | <span data-ttu-id="85698-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="85698-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="85698-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="85698-129">Authorization</span></span> | <span data-ttu-id="85698-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85698-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85698-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85698-132">Request body</span></span>
<span data-ttu-id="85698-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85698-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85698-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85698-134">Response</span></span>
<span data-ttu-id="85698-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85698-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85698-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85698-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="85698-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85698-138">Request</span></span>
<span data-ttu-id="85698-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="85698-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85698-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="85698-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="85698-141">C#</span><span class="sxs-lookup"><span data-stu-id="85698-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85698-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85698-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85698-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85698-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85698-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="85698-144">Response</span></span>

> <span data-ttu-id="85698-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85698-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
