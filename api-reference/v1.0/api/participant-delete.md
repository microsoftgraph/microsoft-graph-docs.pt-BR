---
title: Excluir participante
description: Exclua um participante específico na chamada.
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c08821f723152adb82cde0255d21ea3d8718a8e
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137152"
---
# <a name="delete-participant"></a><span data-ttu-id="61264-103">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="61264-103">Delete participant</span></span>

<span data-ttu-id="61264-104">Excluir um participante específico em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="61264-104">Delete a specific participant in a call.</span></span> <span data-ttu-id="61264-105">Em algumas situações, é apropriado que um aplicativo remova um participante de uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="61264-105">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="61264-106">Esta ação pode ser realizada antes ou depois de o participante responder a chamada.</span><span class="sxs-lookup"><span data-stu-id="61264-106">This action can be done either before or after the participant answers the call.</span></span> <span data-ttu-id="61264-107">Quando um chamador ativo é removido, ele é imediatamente descartado da chamada sem notificação prévia ou após a remoção.</span><span class="sxs-lookup"><span data-stu-id="61264-107">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="61264-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="61264-108">Permissions</span></span>
<span data-ttu-id="61264-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61264-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61264-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61264-111">Permission type</span></span>                        | <span data-ttu-id="61264-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61264-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61264-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61264-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="61264-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="61264-114">Not Supported</span></span>                               |
| <span data-ttu-id="61264-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61264-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61264-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="61264-116">Not Supported</span></span>                               |
| <span data-ttu-id="61264-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61264-117">Application</span></span>                            | <span data-ttu-id="61264-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61264-118">None</span></span>                                        |

<span data-ttu-id="61264-119">A configuração de reunião de aplicativo em nível de locatário é necessária para permitir que um aplicativo chame esta API.</span><span class="sxs-lookup"><span data-stu-id="61264-119">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="61264-120">O administrador do locatário deve chamar o seguinte cmdlet no PowerShell remoto do locatário para conceder a permissão ao aplicativo para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="61264-120">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="61264-121">Para obter mais informações, consulte [set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61264-121">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="61264-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61264-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="61264-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61264-123">Request headers</span></span>
| <span data-ttu-id="61264-124">Nome</span><span class="sxs-lookup"><span data-stu-id="61264-124">Name</span></span>          | <span data-ttu-id="61264-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="61264-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="61264-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="61264-126">Authorization</span></span> | <span data-ttu-id="61264-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61264-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61264-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61264-129">Request body</span></span>
<span data-ttu-id="61264-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61264-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61264-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="61264-131">Response</span></span>
<span data-ttu-id="61264-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61264-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61264-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61264-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61264-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61264-135">Request</span></span>
<span data-ttu-id="61264-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="61264-136">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="61264-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="61264-137">Response</span></span>

> <span data-ttu-id="61264-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61264-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
