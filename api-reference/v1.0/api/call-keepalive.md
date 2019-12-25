---
title: 'Call: keepAlive'
description: Faça uma solicitação para esta API a cada 15 a 45 minutos para garantir que uma chamada em andamento permaneça ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 32de1b3a24c6b37640376cdf7b60289ced5f90f3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865734"
---
# <a name="call-keepalive"></a><span data-ttu-id="f43b1-103">Call: keepAlive</span><span class="sxs-lookup"><span data-stu-id="f43b1-103">call: keepAlive</span></span>

<span data-ttu-id="f43b1-104">Faça uma solicitação para esta API a cada 15 a 45 minutos para garantir que uma chamada em andamento permaneça ativa.</span><span class="sxs-lookup"><span data-stu-id="f43b1-104">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="f43b1-105">Uma chamada que não recebe essa solicitação em 45 minutos é considerada inativa e, subsequentemente, terminará.</span><span class="sxs-lookup"><span data-stu-id="f43b1-105">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="f43b1-106">Pelo menos uma solicitação bem-sucedida deve ser feita em 45 minutos da solicitação anterior ou no início da chamada.</span><span class="sxs-lookup"><span data-stu-id="f43b1-106">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="f43b1-107">Recomendamos que você envie uma solicitação em intervalos de tempo mais curtos (a cada 15 minutos).</span><span class="sxs-lookup"><span data-stu-id="f43b1-107">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="f43b1-108">Certifique-se de que essas solicitações sejam bem-sucedidas para impedir que a chamada saia e termine.</span><span class="sxs-lookup"><span data-stu-id="f43b1-108">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="f43b1-109">A tentativa de enviar uma solicitação para uma chamada já finalizada resultará em um `404 Not-Found` erro.</span><span class="sxs-lookup"><span data-stu-id="f43b1-109">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="f43b1-110">Os recursos relacionados à chamada devem ser limpos no lado do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f43b1-110">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="f43b1-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f43b1-111">Permissions</span></span>
<span data-ttu-id="f43b1-112">Uma das seguintes permissões pode ser necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f43b1-112">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="f43b1-113">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43b1-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f43b1-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f43b1-114">Permission type</span></span> | <span data-ttu-id="f43b1-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f43b1-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f43b1-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f43b1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f43b1-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f43b1-117">Not Supported</span></span>        |
| <span data-ttu-id="f43b1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f43b1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f43b1-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f43b1-119">Not Supported</span></span>        |
| <span data-ttu-id="f43b1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f43b1-120">Application</span></span>     | <span data-ttu-id="f43b1-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f43b1-121">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f43b1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f43b1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="f43b1-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b1-123">Request headers</span></span>
| <span data-ttu-id="f43b1-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f43b1-124">Name</span></span>          | <span data-ttu-id="f43b1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f43b1-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f43b1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f43b1-126">Authorization</span></span> | <span data-ttu-id="f43b1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f43b1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f43b1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b1-129">Request body</span></span>
<span data-ttu-id="f43b1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f43b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f43b1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43b1-131">Response</span></span>
<span data-ttu-id="f43b1-132">Este método retorna um `200 OK` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="f43b1-132">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f43b1-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f43b1-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f43b1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b1-134">Request</span></span>
<span data-ttu-id="f43b1-135">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f43b1-135">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f43b1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f43b1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f43b1-137">C#</span><span class="sxs-lookup"><span data-stu-id="f43b1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f43b1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f43b1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f43b1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f43b1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f43b1-140">Java</span><span class="sxs-lookup"><span data-stu-id="f43b1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f43b1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43b1-141">Response</span></span>
<span data-ttu-id="f43b1-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f43b1-142">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
