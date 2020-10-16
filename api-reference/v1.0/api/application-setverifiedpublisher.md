---
title: 'aplicativo: setVerifiedPublisher'
description: Definir o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9f56a4bf020003f71679c07f380c992b48db491
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471504"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="3d961-103">aplicativo: setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="3d961-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="3d961-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d961-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d961-105">Definir o [verifiedPublisher](../resources/verifiedPublisher.md) em um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="3d961-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="3d961-106">Para obter mais informações, incluindo pré-requisitos para definir um editor verificado, confira [verificação do Publisher](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="3d961-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d961-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d961-107">Permissions</span></span>

|<span data-ttu-id="3d961-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d961-108">Permission type</span></span>      | <span data-ttu-id="3d961-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d961-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d961-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d961-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d961-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d961-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="3d961-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d961-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d961-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3d961-113">Not supported</span></span> |
|<span data-ttu-id="3d961-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d961-114">Application</span></span> | <span data-ttu-id="3d961-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3d961-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d961-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d961-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="3d961-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d961-117">Request headers</span></span>

| <span data-ttu-id="3d961-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3d961-118">Name</span></span>           | <span data-ttu-id="3d961-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d961-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3d961-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d961-120">Authorization</span></span>  | <span data-ttu-id="3d961-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d961-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3d961-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d961-123">Content-Type</span></span>   | <span data-ttu-id="3d961-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d961-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d961-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d961-126">Request body</span></span>

<span data-ttu-id="3d961-127">No corpo da solicitação, forneça as seguintes propriedades obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="3d961-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="3d961-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d961-128">Property</span></span>     | <span data-ttu-id="3d961-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d961-129">Type</span></span>   |<span data-ttu-id="3d961-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d961-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3d961-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="3d961-131">verifiedPublisherId</span></span> | <span data-ttu-id="3d961-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d961-132">string</span></span> | <span data-ttu-id="3d961-133">O MPNID (Microsoft Partner Network ID) do editor verificado a ser definido no aplicativo, na conta do centro de parceiros do Publisher.</span><span class="sxs-lookup"><span data-stu-id="3d961-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="3d961-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d961-134">Response</span></span>

<span data-ttu-id="3d961-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d961-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d961-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d961-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d961-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d961-137">Request</span></span>

<span data-ttu-id="3d961-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d961-138">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="3d961-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d961-139">Response</span></span>

<span data-ttu-id="3d961-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d961-140">The following is an example of the response.</span></span>

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
