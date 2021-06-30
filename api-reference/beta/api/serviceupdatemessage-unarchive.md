---
title: 'serviceUpdateMessage: unarchive'
description: Desaconsuclear uma lista de mensagens de atualização de serviço para o usuário in-loco.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 38144a2f3e6512631f47a22ebecdf7a41e70a417
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209118"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="92ed6-103">serviceUpdateMessage: unarchive</span><span class="sxs-lookup"><span data-stu-id="92ed6-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="92ed6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ed6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ed6-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="92ed6-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="92ed6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92ed6-106">Permissions</span></span>
<span data-ttu-id="92ed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ed6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92ed6-109">Permission type</span></span>|<span data-ttu-id="92ed6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92ed6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92ed6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92ed6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92ed6-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="92ed6-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="92ed6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92ed6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92ed6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92ed6-114">Not supported.</span></span>|
|<span data-ttu-id="92ed6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92ed6-115">Application</span></span>|<span data-ttu-id="92ed6-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="92ed6-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="92ed6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92ed6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="92ed6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed6-118">Request headers</span></span>
|<span data-ttu-id="92ed6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="92ed6-119">Name</span></span>|<span data-ttu-id="92ed6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ed6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="92ed6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="92ed6-121">Authorization</span></span>|<span data-ttu-id="92ed6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ed6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="92ed6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92ed6-124">Content-Type</span></span>|<span data-ttu-id="92ed6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ed6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed6-127">Request body</span></span>
<span data-ttu-id="92ed6-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="92ed6-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="92ed6-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="92ed6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92ed6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="92ed6-130">Parameter</span></span>|<span data-ttu-id="92ed6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ed6-131">Type</span></span>|<span data-ttu-id="92ed6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ed6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ed6-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="92ed6-133">messageIds</span></span>|<span data-ttu-id="92ed6-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92ed6-134">String collection</span></span>|<span data-ttu-id="92ed6-135">Lista de IDs de mensagens a ser desarquivada.</span><span class="sxs-lookup"><span data-stu-id="92ed6-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="92ed6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ed6-136">Response</span></span>

<span data-ttu-id="92ed6-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um valor Boolean no corpo da `true` resposta.</span><span class="sxs-lookup"><span data-stu-id="92ed6-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="92ed6-138">Caso contrário, `false` retornará no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92ed6-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ed6-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92ed6-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="92ed6-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed6-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="92ed6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="92ed6-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92ed6-142">C#</span><span class="sxs-lookup"><span data-stu-id="92ed6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceupdatemessage-unarchive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92ed6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92ed6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceupdatemessage-unarchive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92ed6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92ed6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceupdatemessage-unarchive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92ed6-145">Java</span><span class="sxs-lookup"><span data-stu-id="92ed6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceupdatemessage-unarchive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="92ed6-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ed6-146">Response</span></span>
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
