---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89da0fa3f569743dfe9bae31f2a30a00438794f2
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667609"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="1756d-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="1756d-103">Get certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1756d-104">Obter as propriedades de um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1756d-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1756d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1756d-105">Permissions</span></span>

<span data-ttu-id="1756d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1756d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1756d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1756d-108">Permission type</span></span>                        | <span data-ttu-id="1756d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1756d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1756d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1756d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1756d-111">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1756d-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="1756d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1756d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1756d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1756d-113">Not supported.</span></span> |
| <span data-ttu-id="1756d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1756d-114">Application</span></span>    | <span data-ttu-id="1756d-115">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1756d-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1756d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1756d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1756d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1756d-117">Request headers</span></span>

| <span data-ttu-id="1756d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1756d-118">Name</span></span>      |<span data-ttu-id="1756d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1756d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1756d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1756d-120">Authorization</span></span> | <span data-ttu-id="1756d-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1756d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1756d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1756d-122">Request body</span></span>

<span data-ttu-id="1756d-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1756d-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1756d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="1756d-124">Response</span></span>

<span data-ttu-id="1756d-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1756d-125">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1756d-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1756d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1756d-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1756d-127">Request</span></span>

<span data-ttu-id="1756d-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1756d-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```

### <a name="response"></a><span data-ttu-id="1756d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1756d-129">Response</span></span>

<span data-ttu-id="1756d-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1756d-130">The following is an example of the response.</span></span>

> <span data-ttu-id="1756d-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1756d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificateRevocationListUrl": "CRLUrl-value",
      "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->