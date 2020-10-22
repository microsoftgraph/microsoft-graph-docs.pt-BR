---
title: 'aplicativo: unsetVerifiedPublisher'
description: Desmarcar o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dca739f5086e10fecdfba56cfd1338a9230b4d4d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635506"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="18252-103">aplicativo: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="18252-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="18252-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18252-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18252-105">Desmarque a [verifiedPublisher](../resources/verifiedPublisher.md) definida anteriormente em um [aplicativo](../resources/application.md), removendo todas as propriedades verificadas do Publisher.</span><span class="sxs-lookup"><span data-stu-id="18252-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="18252-106">Para obter mais informações, consulte [Publisher Verification](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="18252-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="18252-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="18252-107">Permissions</span></span>

|<span data-ttu-id="18252-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18252-108">Permission type</span></span>      | <span data-ttu-id="18252-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18252-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18252-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18252-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18252-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18252-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="18252-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18252-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18252-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="18252-113">Not supported</span></span> |
|<span data-ttu-id="18252-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18252-114">Application</span></span> | <span data-ttu-id="18252-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="18252-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="18252-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18252-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="18252-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18252-117">Request headers</span></span>

| <span data-ttu-id="18252-118">Nome</span><span class="sxs-lookup"><span data-stu-id="18252-118">Name</span></span>           | <span data-ttu-id="18252-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="18252-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="18252-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="18252-120">Authorization</span></span>  | <span data-ttu-id="18252-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18252-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18252-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18252-123">Request body</span></span>

<span data-ttu-id="18252-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18252-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18252-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="18252-125">Response</span></span>

<span data-ttu-id="18252-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18252-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18252-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18252-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="18252-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18252-128">Request</span></span>

<span data-ttu-id="18252-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18252-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18252-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="18252-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="18252-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18252-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18252-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18252-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18252-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="18252-133">Response</span></span>

<span data-ttu-id="18252-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18252-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: db9f2d4d-e668-4eda-9d88-776b6ca6ca20
2020-09-09 21:29:08 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
