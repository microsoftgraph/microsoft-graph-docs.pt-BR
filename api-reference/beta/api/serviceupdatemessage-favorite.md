---
title: 'serviceUpdateMessage: favorite'
description: Altere o status de uma lista de mensagens de atualização de serviço para favoritos para o usuário inscrevado.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 4d15bba0aa3f2aa498a7b6849518cc2155a2369d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209188"
---
# <a name="serviceupdatemessage-favorite"></a><span data-ttu-id="cdc8f-103">serviceUpdateMessage: favorite</span><span class="sxs-lookup"><span data-stu-id="cdc8f-103">serviceUpdateMessage: favorite</span></span>
<span data-ttu-id="cdc8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc8f-105">Altere o status de uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como favorito para o usuário que está assinado.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-105">Change the status of a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) to favorite for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc8f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdc8f-106">Permissions</span></span>
<span data-ttu-id="cdc8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc8f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdc8f-109">Permission type</span></span>|<span data-ttu-id="cdc8f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdc8f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc8f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdc8f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdc8f-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="cdc8f-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="cdc8f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdc8f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdc8f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-114">Not supported.</span></span>|
|<span data-ttu-id="cdc8f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdc8f-115">Application</span></span>|<span data-ttu-id="cdc8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdc8f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc8f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/favorite
```

## <a name="request-headers"></a><span data-ttu-id="cdc8f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc8f-118">Request headers</span></span>
|<span data-ttu-id="cdc8f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cdc8f-119">Name</span></span>|<span data-ttu-id="cdc8f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc8f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cdc8f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdc8f-121">Authorization</span></span>|<span data-ttu-id="cdc8f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cdc8f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdc8f-124">Content-Type</span></span>|<span data-ttu-id="cdc8f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc8f-127">Request body</span></span>
<span data-ttu-id="cdc8f-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="cdc8f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cdc8f-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cdc8f-130">Parameter</span></span>|<span data-ttu-id="cdc8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdc8f-131">Type</span></span>|<span data-ttu-id="cdc8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc8f-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="cdc8f-133">messageIds</span></span>|<span data-ttu-id="cdc8f-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdc8f-134">String collection</span></span>|<span data-ttu-id="cdc8f-135">Lista de IDs de mensagem para salvar como favorito.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-135">List of message IDs to save as favorite.</span></span>|

## <a name="response"></a><span data-ttu-id="cdc8f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc8f-136">Response</span></span>

<span data-ttu-id="cdc8f-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um valor Boolean no corpo da `true` resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="cdc8f-138">Caso contrário, `false` retornará no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc8f-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc8f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdc8f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdc8f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc8f-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cdc8f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc8f-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cdc8f-142">C#</span><span class="sxs-lookup"><span data-stu-id="cdc8f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceupdatemessage-favorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc8f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc8f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceupdatemessage-favorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc8f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc8f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceupdatemessage-favorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc8f-145">Java</span><span class="sxs-lookup"><span data-stu-id="cdc8f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceupdatemessage-favorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdc8f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc8f-146">Response</span></span>
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
