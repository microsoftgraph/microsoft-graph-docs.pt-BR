---
title: 'serviceUpdateMessage: favorite'
description: Altere o status de uma lista de mensagens de atualização de serviço para favoritos para o usuário inscrevado.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 5838b8c395db539f06aad31ef7794eda2f8587ad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107765"
---
# <a name="serviceupdatemessage-favorite"></a><span data-ttu-id="7576c-103">serviceUpdateMessage: favorite</span><span class="sxs-lookup"><span data-stu-id="7576c-103">serviceUpdateMessage: favorite</span></span>
<span data-ttu-id="7576c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7576c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7576c-105">Altere o status de uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como favorito para o usuário que está assinado.</span><span class="sxs-lookup"><span data-stu-id="7576c-105">Change the status of a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) to favorite for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7576c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7576c-106">Permissions</span></span>
<span data-ttu-id="7576c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7576c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7576c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7576c-109">Permission type</span></span>|<span data-ttu-id="7576c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7576c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7576c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7576c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7576c-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="7576c-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="7576c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7576c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7576c-114">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="7576c-114">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="7576c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7576c-115">Application</span></span>|<span data-ttu-id="7576c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7576c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7576c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7576c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/favorite
```

## <a name="request-headers"></a><span data-ttu-id="7576c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7576c-118">Request headers</span></span>
|<span data-ttu-id="7576c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7576c-119">Name</span></span>|<span data-ttu-id="7576c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7576c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7576c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7576c-121">Authorization</span></span>|<span data-ttu-id="7576c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7576c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7576c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7576c-124">Content-Type</span></span>|<span data-ttu-id="7576c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7576c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7576c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7576c-127">Request body</span></span>
<span data-ttu-id="7576c-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7576c-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="7576c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7576c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7576c-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7576c-130">Parameter</span></span>|<span data-ttu-id="7576c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7576c-131">Type</span></span>|<span data-ttu-id="7576c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7576c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7576c-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="7576c-133">messageIds</span></span>|<span data-ttu-id="7576c-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7576c-134">String collection</span></span>|<span data-ttu-id="7576c-135">Lista de IDs de mensagem para salvar como favorito.</span><span class="sxs-lookup"><span data-stu-id="7576c-135">List of message IDs to save as favorite.</span></span>|

## <a name="response"></a><span data-ttu-id="7576c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7576c-136">Response</span></span>

<span data-ttu-id="7576c-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um valor Boolean no corpo da `true` resposta.</span><span class="sxs-lookup"><span data-stu-id="7576c-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="7576c-138">Caso contrário, `false` retornará no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7576c-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7576c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7576c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7576c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7576c-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_favorite"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/favorite
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a><span data-ttu-id="7576c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7576c-141">Response</span></span>
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
