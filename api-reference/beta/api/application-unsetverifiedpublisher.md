---
title: 'application: unsetVerifiedPublisher'
description: Desmarcar o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7560d9935a2cf35bcf67637ce2353932ba522d2b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759913"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="50474-103">application: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="50474-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="50474-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50474-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50474-105">Desajuste [o verificadoPublisher](../resources/verifiedPublisher.md) definido anteriormente em um [aplicativo,](../resources/application.md)removendo todas as propriedades do editor verificadas.</span><span class="sxs-lookup"><span data-stu-id="50474-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="50474-106">Para obter mais informações, consulte [Verificação do Publisher](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="50474-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="50474-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="50474-107">Permissions</span></span>

|<span data-ttu-id="50474-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50474-108">Permission type</span></span>      | <span data-ttu-id="50474-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50474-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50474-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50474-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50474-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50474-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="50474-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50474-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50474-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="50474-113">Not supported</span></span> |
|<span data-ttu-id="50474-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50474-114">Application</span></span> | <span data-ttu-id="50474-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="50474-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="50474-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50474-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="50474-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50474-117">Request headers</span></span>

| <span data-ttu-id="50474-118">Nome</span><span class="sxs-lookup"><span data-stu-id="50474-118">Name</span></span>           | <span data-ttu-id="50474-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50474-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="50474-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="50474-120">Authorization</span></span>  | <span data-ttu-id="50474-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50474-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50474-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50474-123">Request body</span></span>

<span data-ttu-id="50474-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50474-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50474-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="50474-125">Response</span></span>

<span data-ttu-id="50474-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50474-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50474-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50474-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="50474-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50474-128">Request</span></span>

<span data-ttu-id="50474-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50474-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50474-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="50474-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="50474-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50474-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50474-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50474-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50474-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="50474-133">Response</span></span>

<span data-ttu-id="50474-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50474-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: b0ed721f-7e6a-446c-89bc-2d03e1744dfe
2020-09-09 21:26:11 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
