---
title: 'application: setVerifiedPublisher'
description: Definir o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ff0558f8618020eca6437d7528f1f6d0f17eafa6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761146"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="df784-103">application: setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="df784-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="df784-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df784-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df784-105">De definir [o verificadoPublisher](../resources/verifiedPublisher.md) em um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="df784-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="df784-106">Para obter mais informações, incluindo pré-requisitos para definir um editor verificado, consulte [Verificação do Publisher](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="df784-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="df784-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="df784-107">Permissions</span></span>

|<span data-ttu-id="df784-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df784-108">Permission type</span></span>      | <span data-ttu-id="df784-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df784-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df784-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df784-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df784-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df784-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="df784-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df784-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df784-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="df784-113">Not supported</span></span> |
|<span data-ttu-id="df784-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df784-114">Application</span></span> | <span data-ttu-id="df784-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="df784-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="df784-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df784-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="df784-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df784-117">Request headers</span></span>

| <span data-ttu-id="df784-118">Nome</span><span class="sxs-lookup"><span data-stu-id="df784-118">Name</span></span>           | <span data-ttu-id="df784-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="df784-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="df784-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="df784-120">Authorization</span></span>  | <span data-ttu-id="df784-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df784-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df784-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df784-123">Content-Type</span></span>   | <span data-ttu-id="df784-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df784-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df784-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df784-126">Request body</span></span>

<span data-ttu-id="df784-127">No corpo da solicitação, forneça as seguintes propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="df784-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="df784-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df784-128">Property</span></span>     | <span data-ttu-id="df784-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="df784-129">Type</span></span>   |<span data-ttu-id="df784-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="df784-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="df784-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="df784-131">verifiedPublisherId</span></span> | <span data-ttu-id="df784-132">string</span><span class="sxs-lookup"><span data-stu-id="df784-132">string</span></span> | <span data-ttu-id="df784-133">A ID da Rede de Parceiros da Microsoft (MPNID) do editor verificado a ser definida no aplicativo, a partir da conta do Partner Center do editor.</span><span class="sxs-lookup"><span data-stu-id="df784-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="df784-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df784-134">Response</span></span>

<span data-ttu-id="df784-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df784-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df784-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df784-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="df784-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df784-137">Request</span></span>

<span data-ttu-id="df784-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df784-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df784-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="df784-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```
# <a name="javascript"></a>[<span data-ttu-id="df784-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df784-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df784-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="df784-141">Response</span></span>

<span data-ttu-id="df784-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df784-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8c7a28dd-cebd-4dc0-b195-b2c7476e7a65
2020-09-09 21:28:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
