---
title: 'serviceUpdateMessage: unarchive'
description: Desaconsuclear uma lista de mensagens de atualização de serviço para o usuário in-loco.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: c92f5af0b718bcf57f4e0e685046e54b5d55e033
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151703"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="ec085-103">serviceUpdateMessage: unarchive</span><span class="sxs-lookup"><span data-stu-id="ec085-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="ec085-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec085-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec085-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="ec085-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec085-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec085-106">Permissions</span></span>
<span data-ttu-id="ec085-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec085-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec085-109">Permission type</span></span>|<span data-ttu-id="ec085-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec085-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec085-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec085-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec085-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="ec085-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="ec085-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec085-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec085-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec085-114">Not supported.</span></span>|
|<span data-ttu-id="ec085-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec085-115">Application</span></span>|<span data-ttu-id="ec085-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ec085-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec085-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec085-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="ec085-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec085-118">Request headers</span></span>
|<span data-ttu-id="ec085-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ec085-119">Name</span></span>|<span data-ttu-id="ec085-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec085-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec085-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec085-121">Authorization</span></span>|<span data-ttu-id="ec085-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec085-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ec085-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec085-124">Content-Type</span></span>|<span data-ttu-id="ec085-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec085-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec085-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec085-127">Request body</span></span>
<span data-ttu-id="ec085-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ec085-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="ec085-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ec085-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ec085-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ec085-130">Parameter</span></span>|<span data-ttu-id="ec085-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec085-131">Type</span></span>|<span data-ttu-id="ec085-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec085-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec085-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="ec085-133">messageIds</span></span>|<span data-ttu-id="ec085-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec085-134">String collection</span></span>|<span data-ttu-id="ec085-135">Lista de IDs de mensagens a ser desarquivada.</span><span class="sxs-lookup"><span data-stu-id="ec085-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="ec085-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec085-136">Response</span></span>

<span data-ttu-id="ec085-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um valor Boolean no corpo da `true` resposta.</span><span class="sxs-lookup"><span data-stu-id="ec085-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="ec085-138">Caso contrário, `false` retornará no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec085-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec085-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec085-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec085-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec085-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_unarchive"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/unarchive
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```


### <a name="response"></a><span data-ttu-id="ec085-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec085-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```