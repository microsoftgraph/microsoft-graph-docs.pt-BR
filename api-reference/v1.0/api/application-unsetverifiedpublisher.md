---
title: 'aplicativo: unsetVerifiedPublisher'
description: Desmarcar o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee598fc37ad3aa2abc8dac1a7980b29a53e41029
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471503"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="02fad-103">aplicativo: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="02fad-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="02fad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02fad-105">Desmarque a [verifiedPublisher](../resources/verifiedPublisher.md) definida anteriormente em um [aplicativo](../resources/application.md), removendo todas as propriedades verificadas do Publisher.</span><span class="sxs-lookup"><span data-stu-id="02fad-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="02fad-106">Para obter mais informações, consulte [Publisher Verification](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="02fad-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="02fad-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="02fad-107">Permissions</span></span>

|<span data-ttu-id="02fad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02fad-108">Permission type</span></span>      | <span data-ttu-id="02fad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02fad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02fad-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02fad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02fad-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02fad-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="02fad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02fad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02fad-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="02fad-113">Not supported</span></span> |
|<span data-ttu-id="02fad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02fad-114">Application</span></span> | <span data-ttu-id="02fad-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="02fad-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="02fad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02fad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="02fad-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02fad-117">Request headers</span></span>

| <span data-ttu-id="02fad-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02fad-118">Name</span></span>           | <span data-ttu-id="02fad-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fad-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="02fad-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02fad-120">Authorization</span></span>  | <span data-ttu-id="02fad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02fad-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02fad-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02fad-123">Request body</span></span>

<span data-ttu-id="02fad-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02fad-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02fad-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fad-125">Response</span></span>

<span data-ttu-id="02fad-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02fad-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02fad-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02fad-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="02fad-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02fad-128">Request</span></span>

<span data-ttu-id="02fad-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02fad-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a><span data-ttu-id="02fad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fad-130">Response</span></span>

<span data-ttu-id="02fad-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02fad-131">The following is an example of the response.</span></span>

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
