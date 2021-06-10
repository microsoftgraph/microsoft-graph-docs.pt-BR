---
title: 'channel: provisionEmail'
description: Provisione o email de um canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b2e619970c0cdadd574a4873cb3231a88934a087
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869621"
---
# <a name="channel-provisionemail"></a><span data-ttu-id="5ac9e-103">channel: provisionEmail</span><span class="sxs-lookup"><span data-stu-id="5ac9e-103">channel: provisionEmail</span></span>

<span data-ttu-id="5ac9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ac9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ac9e-105">Provisionar um endereço de email para um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5ac9e-105">Provision an email address for a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="5ac9e-106">Microsoft Teams não provisiona automaticamente um endereço de email para um canal por padrão.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-106">Microsoft Teams does not automatically provision an email address for a channel by default.</span></span> <span data-ttu-id="5ac9e-107">Para ter Teams provisionar um endereço de email, você pode chamar **provisionEmail** ou por meio da interface de usuário do Teams, selecione Obter endereço de **email**, que dispara Teams para gerar um endereço de email se ele ainda não tiver provisionado um.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-107">To have Teams provision an email address, you can call **provisionEmail**, or through the Teams user interface, select **Get email address**, which triggers Teams to generate an email address if it has not already provisioned one.</span></span>

<span data-ttu-id="5ac9e-108">Para remover o endereço de email provisionado de um canal, use o [método removeEmail.](channel-removeemail.md)</span><span class="sxs-lookup"><span data-stu-id="5ac9e-108">To remove a channel's provisioned email address, use the [removeEmail](channel-removeemail.md) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ac9e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5ac9e-109">Permissions</span></span>

<span data-ttu-id="5ac9e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ac9e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ac9e-112">Permission type</span></span>                        | <span data-ttu-id="5ac9e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ac9e-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5ac9e-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ac9e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ac9e-115">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac9e-115">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="5ac9e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ac9e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ac9e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-117">Not supported.</span></span>                              |
| <span data-ttu-id="5ac9e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ac9e-118">Application</span></span>                            | <span data-ttu-id="5ac9e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="5ac9e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ac9e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a><span data-ttu-id="5ac9e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac9e-121">Request headers</span></span>
| <span data-ttu-id="5ac9e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ac9e-122">Header</span></span>        | <span data-ttu-id="5ac9e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5ac9e-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5ac9e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ac9e-124">Authorization</span></span> | <span data-ttu-id="5ac9e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ac9e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac9e-127">Request body</span></span>

<span data-ttu-id="5ac9e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ac9e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac9e-129">Response</span></span>

<span data-ttu-id="5ac9e-130">Se o email do canal for provisionado com êxito, este método retornará um código de resposta e um `200 OK` [objeto provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-130">If the channel's email is provisioned successfully, this method returns a `200 OK` response code and a [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) object in the response body.</span></span> <span data-ttu-id="5ac9e-131">O endereço de email provisionado está na **propriedade email.**</span><span class="sxs-lookup"><span data-stu-id="5ac9e-131">The provisioned email address is in the **email** property.</span></span>

## <a name="example"></a><span data-ttu-id="5ac9e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ac9e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ac9e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac9e-133">Request</span></span>
<span data-ttu-id="5ac9e-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ac9e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ac9e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```
# <a name="c"></a>[<span data-ttu-id="5ac9e-136">C#</span><span class="sxs-lookup"><span data-stu-id="5ac9e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-provisionemail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ac9e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ac9e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-provisionemail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ac9e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ac9e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-provisionemail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ac9e-139">Java</span><span class="sxs-lookup"><span data-stu-id="5ac9e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-provisionemail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ac9e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac9e-140">Response</span></span>
<span data-ttu-id="5ac9e-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-141">The following is an example of a response.</span></span>
<span data-ttu-id="5ac9e-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ac9e-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


