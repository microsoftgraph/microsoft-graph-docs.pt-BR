---
title: 'aplicativo: unsetVerifiedPublisher'
description: Remover a desdefinição do fornecedor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f904a4b13e162dc503765b03d676319d3d0a510
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471543"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="9b1e0-103">aplicativo: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="9b1e0-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="9b1e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b1e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b1e0-105">Desmarque o [verifiedPublisher](../resources/verifiedPublisher.md) definido anteriormente em um [aplicativo](../resources/application.md), removendo todas as propriedades verificadas do Publisher.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="9b1e0-106">Para obter mais informações, consulte [Publisher Verification](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="9b1e0-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b1e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b1e0-107">Permissions</span></span>

|<span data-ttu-id="9b1e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b1e0-108">Permission type</span></span>      | <span data-ttu-id="9b1e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b1e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b1e0-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b1e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b1e0-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b1e0-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="9b1e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b1e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b1e0-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9b1e0-113">Not supported</span></span> |
|<span data-ttu-id="9b1e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b1e0-114">Application</span></span> | <span data-ttu-id="9b1e0-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9b1e0-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b1e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b1e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="9b1e0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b1e0-117">Request headers</span></span>

| <span data-ttu-id="9b1e0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b1e0-118">Name</span></span>           | <span data-ttu-id="9b1e0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b1e0-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="9b1e0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b1e0-120">Authorization</span></span>  | <span data-ttu-id="9b1e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b1e0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b1e0-123">Request body</span></span>

<span data-ttu-id="9b1e0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b1e0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b1e0-125">Response</span></span>

<span data-ttu-id="9b1e0-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9b1e0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b1e0-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b1e0-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b1e0-128">Request</span></span>

<span data-ttu-id="9b1e0-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a><span data-ttu-id="9b1e0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b1e0-130">Response</span></span>

<span data-ttu-id="9b1e0-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b1e0-131">The following is an example of the response.</span></span>

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
