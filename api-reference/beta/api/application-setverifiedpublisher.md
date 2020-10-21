---
title: 'aplicativo: setVerifiedPublisher'
description: Definir o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3aa6156ca95e1d75376ac24be9883aa0ed3db04e
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634575"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="a05cc-103">aplicativo: setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="a05cc-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="a05cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a05cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a05cc-105">Definir o [verifiedPublisher](../resources/verifiedPublisher.md) em um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="a05cc-105">Set the the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="a05cc-106">Para obter mais informações, incluindo pré-requisitos para definir um editor verificado, confira [verificação do Publisher](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="a05cc-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="a05cc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a05cc-107">Permissions</span></span>

|<span data-ttu-id="a05cc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a05cc-108">Permission type</span></span>      | <span data-ttu-id="a05cc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a05cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a05cc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a05cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a05cc-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a05cc-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="a05cc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a05cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a05cc-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a05cc-113">Not supported</span></span> |
|<span data-ttu-id="a05cc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a05cc-114">Application</span></span> | <span data-ttu-id="a05cc-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a05cc-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="a05cc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05cc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="a05cc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a05cc-117">Request headers</span></span>

| <span data-ttu-id="a05cc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a05cc-118">Name</span></span>           | <span data-ttu-id="a05cc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a05cc-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a05cc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a05cc-120">Authorization</span></span>  | <span data-ttu-id="a05cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a05cc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a05cc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a05cc-123">Content-Type</span></span>   | <span data-ttu-id="a05cc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a05cc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a05cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a05cc-126">Request body</span></span>

<span data-ttu-id="a05cc-127">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="a05cc-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="a05cc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a05cc-128">Property</span></span>     | <span data-ttu-id="a05cc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a05cc-129">Type</span></span>   |<span data-ttu-id="a05cc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a05cc-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a05cc-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="a05cc-131">verifiedPublisherId</span></span> | <span data-ttu-id="a05cc-132">string</span><span class="sxs-lookup"><span data-stu-id="a05cc-132">string</span></span> | <span data-ttu-id="a05cc-133">O MPNID (Microsoft Partner Network ID) do editor verificado a ser definido no aplicativo, na conta do centro de parceiros do Publisher.</span><span class="sxs-lookup"><span data-stu-id="a05cc-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="a05cc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05cc-134">Response</span></span>

<span data-ttu-id="a05cc-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a05cc-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a05cc-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a05cc-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a05cc-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a05cc-137">Request</span></span>

<span data-ttu-id="a05cc-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a05cc-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a05cc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05cc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a05cc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05cc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a05cc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05cc-141">Response</span></span>

<span data-ttu-id="a05cc-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a05cc-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: e7beba93-bb0b-42ea-96c8-231aa61d755e
2020-09-09 21:16:07 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
