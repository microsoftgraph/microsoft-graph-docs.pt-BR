---
title: 'channel: provisionEmail'
description: Provisione o email de um canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35865ff1b44fad5bc66951df571dbd5252a363df
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813222"
---
# <a name="channel-provisionemail"></a><span data-ttu-id="ff565-103">channel: provisionEmail</span><span class="sxs-lookup"><span data-stu-id="ff565-103">channel: provisionEmail</span></span>

<span data-ttu-id="ff565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff565-105">Provisionar um endereço de email para um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ff565-105">Provision an email address for a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="ff565-106">Microsoft Teams não provisiona automaticamente um endereço de email para um canal por padrão.</span><span class="sxs-lookup"><span data-stu-id="ff565-106">Microsoft Teams does not automatically provision an email address for a channel by default.</span></span> <span data-ttu-id="ff565-107">Para ter Teams provisionar um endereço de email, você pode chamar **provisionEmail** ou por meio da interface de usuário do Teams, selecione Obter endereço de **email**, que dispara Teams para gerar um endereço de email se ele ainda não tiver provisionado um.</span><span class="sxs-lookup"><span data-stu-id="ff565-107">To have Teams provision an email address, you can call **provisionEmail**, or through the Teams user interface, select **Get email address**, which triggers Teams to generate an email address if it has not already provisioned one.</span></span>

<span data-ttu-id="ff565-108">Para remover o endereço de email provisionado de um canal, use o [método removeEmail.](channel-removeemail.md)</span><span class="sxs-lookup"><span data-stu-id="ff565-108">To remove a channel's provisioned email address, use the [removeEmail](channel-removeemail.md) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff565-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff565-109">Permissions</span></span>

<span data-ttu-id="ff565-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff565-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff565-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff565-112">Permission type</span></span>                        | <span data-ttu-id="ff565-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff565-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ff565-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff565-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff565-115">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff565-115">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="ff565-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff565-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff565-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff565-117">Not supported.</span></span>                              |
| <span data-ttu-id="ff565-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff565-118">Application</span></span>                            | <span data-ttu-id="ff565-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff565-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="ff565-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff565-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a><span data-ttu-id="ff565-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff565-121">Request headers</span></span>
| <span data-ttu-id="ff565-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff565-122">Header</span></span>        | <span data-ttu-id="ff565-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ff565-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ff565-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff565-124">Authorization</span></span> | <span data-ttu-id="ff565-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff565-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff565-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff565-127">Request body</span></span>

<span data-ttu-id="ff565-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff565-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff565-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff565-129">Response</span></span>

<span data-ttu-id="ff565-130">Se o email do canal for provisionado com êxito, este método retornará um código de resposta e um `200 OK` [objeto provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff565-130">If the channel's email is provisioned successfully, this method returns a `200 OK` response code and a [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) object in the response body.</span></span> <span data-ttu-id="ff565-131">O endereço de email provisionado está na **propriedade email.**</span><span class="sxs-lookup"><span data-stu-id="ff565-131">The provisioned email address is in the **email** property.</span></span>

## <a name="example"></a><span data-ttu-id="ff565-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff565-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff565-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff565-133">Request</span></span>
<span data-ttu-id="ff565-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff565-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```

### <a name="response"></a><span data-ttu-id="ff565-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff565-135">Response</span></span>
<span data-ttu-id="ff565-136">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ff565-136">The following is an example of a response.</span></span>
<span data-ttu-id="ff565-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff565-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
    "email": "1df8f174.teamsgraph.onmicrosoft.com@amer.teams.ms"
}
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Provision channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


