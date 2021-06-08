---
title: 'channel: removeEmail'
description: Remova o email provisionado de um canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4608538cf136ba4f53a960183bc0b3f4bd7fc269
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813220"
---
# <a name="channel-removeemail"></a><span data-ttu-id="42f4f-103">channel: removeEmail</span><span class="sxs-lookup"><span data-stu-id="42f4f-103">channel: removeEmail</span></span>

<span data-ttu-id="42f4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f4f-105">Remova o endereço de email provisionado de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="42f4f-105">Remove the provisioned email address of a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="42f4f-106">Você só poderá remover um endereço de email se ele tiver sido provisionado usando o [método provisionEmail](channel-provisionemail.md) ou por meio do Microsoft Teams cliente.</span><span class="sxs-lookup"><span data-stu-id="42f4f-106">You can remove an email address only if it was provisioned using the [provisionEmail](channel-provisionemail.md) method or through the Microsoft Teams client.</span></span>

## <a name="permissions"></a><span data-ttu-id="42f4f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="42f4f-107">Permissions</span></span>

<span data-ttu-id="42f4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42f4f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42f4f-110">Permission type</span></span>                        | <span data-ttu-id="42f4f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42f4f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="42f4f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42f4f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="42f4f-113">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f4f-113">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="42f4f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42f4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f4f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42f4f-115">Not supported.</span></span>                              |
| <span data-ttu-id="42f4f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42f4f-116">Application</span></span>                            | <span data-ttu-id="42f4f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42f4f-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="42f4f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42f4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/removeEmail
```
## <a name="request-headers"></a><span data-ttu-id="42f4f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4f-119">Request headers</span></span>
| <span data-ttu-id="42f4f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42f4f-120">Header</span></span>        | <span data-ttu-id="42f4f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42f4f-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="42f4f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42f4f-122">Authorization</span></span> | <span data-ttu-id="42f4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42f4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f4f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4f-125">Request body</span></span>

<span data-ttu-id="42f4f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42f4f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42f4f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f4f-127">Response</span></span>

<span data-ttu-id="42f4f-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42f4f-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42f4f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42f4f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="42f4f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42f4f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_removeemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail
```

### <a name="response"></a><span data-ttu-id="42f4f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f4f-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


