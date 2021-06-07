---
title: 'call: keepAlive'
description: Faça uma solicitação a essa API a cada 15 a 45 minutos para garantir que uma chamada contínua permaneça viva.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a2561e33810264587951ae3b20a19507bf6e6abf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788119"
---
# <a name="call-keepalive"></a><span data-ttu-id="26ecf-103">call: keepAlive</span><span class="sxs-lookup"><span data-stu-id="26ecf-103">call: keepAlive</span></span>

<span data-ttu-id="26ecf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ecf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26ecf-105">Faça uma solicitação a essa API a cada 15 a 45 minutos para garantir que uma chamada contínua permaneça ativa.</span><span class="sxs-lookup"><span data-stu-id="26ecf-105">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="26ecf-106">Uma chamada que não recebe essa solicitação dentro de 45 minutos é considerada inativa e termina subsequentemente.</span><span class="sxs-lookup"><span data-stu-id="26ecf-106">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="26ecf-107">Pelo menos uma solicitação bem-sucedida deve ser feita dentro de 45 minutos após a solicitação anterior ou o início da chamada.</span><span class="sxs-lookup"><span data-stu-id="26ecf-107">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="26ecf-108">Recomendamos que você envie uma solicitação em intervalos de tempo mais curtos (a cada 15 minutos).</span><span class="sxs-lookup"><span data-stu-id="26ecf-108">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="26ecf-109">Certifique-se de que essas solicitações sejam bem-sucedidas para impedir que a chamada seja terminada e fora do tempo.</span><span class="sxs-lookup"><span data-stu-id="26ecf-109">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="26ecf-110">Tentar enviar uma solicitação para uma chamada que já terminou resultará em um `404 Not-Found` erro.</span><span class="sxs-lookup"><span data-stu-id="26ecf-110">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="26ecf-111">Os recursos relacionados à chamada devem ser limpos no lado do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26ecf-111">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="26ecf-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="26ecf-112">Permissions</span></span>
<span data-ttu-id="26ecf-113">Uma das seguintes permissões pode ser necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="26ecf-113">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="26ecf-114">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ecf-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26ecf-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ecf-115">Permission type</span></span> | <span data-ttu-id="26ecf-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26ecf-116">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="26ecf-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ecf-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="26ecf-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="26ecf-118">Not Supported</span></span>        |
| <span data-ttu-id="26ecf-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ecf-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ecf-120">Não suportado</span><span class="sxs-lookup"><span data-stu-id="26ecf-120">Not Supported</span></span>        |
| <span data-ttu-id="26ecf-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ecf-121">Application</span></span>     | <span data-ttu-id="26ecf-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="26ecf-122">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="26ecf-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ecf-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="26ecf-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26ecf-124">Request headers</span></span>
| <span data-ttu-id="26ecf-125">Nome</span><span class="sxs-lookup"><span data-stu-id="26ecf-125">Name</span></span>          | <span data-ttu-id="26ecf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ecf-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="26ecf-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ecf-127">Authorization</span></span> | <span data-ttu-id="26ecf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26ecf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26ecf-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ecf-130">Request body</span></span>
<span data-ttu-id="26ecf-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26ecf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26ecf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ecf-132">Response</span></span>
<span data-ttu-id="26ecf-133">Este método retorna um `200 OK` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="26ecf-133">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26ecf-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26ecf-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26ecf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ecf-135">Request</span></span>
<span data-ttu-id="26ecf-136">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ecf-136">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26ecf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="26ecf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="c"></a>[<span data-ttu-id="26ecf-138">C#</span><span class="sxs-lookup"><span data-stu-id="26ecf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26ecf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26ecf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26ecf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26ecf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26ecf-141">Java</span><span class="sxs-lookup"><span data-stu-id="26ecf-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="26ecf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ecf-142">Response</span></span>
<span data-ttu-id="26ecf-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="26ecf-143">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

