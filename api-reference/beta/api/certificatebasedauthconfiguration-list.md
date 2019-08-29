---
title: Listar certificateBasedAuthConfigurations
description: Obtenha uma lista de objetos certificatebasedauthconfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7452f081725dab0b98c7f45529bc9416018df2c3
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667610"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="8f08a-103">Listar certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="8f08a-103">List certificateBasedAuthConfigurations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f08a-104">Obtenha uma lista de objetos [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8f08a-104">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="8f08a-105">Apenas uma única instância do certificateBasedAuthConfiguration pode existir na coleção.</span><span class="sxs-lookup"><span data-stu-id="8f08a-105">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="8f08a-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="8f08a-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f08a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f08a-107">Permissions</span></span>

<span data-ttu-id="8f08a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f08a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f08a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f08a-110">Permission type</span></span>                        | <span data-ttu-id="8f08a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f08a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f08a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f08a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f08a-113">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8f08a-113">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="8f08a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f08a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f08a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f08a-115">Not supported.</span></span> |
| <span data-ttu-id="8f08a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f08a-116">Application</span></span>    | <span data-ttu-id="8f08a-117">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8f08a-117">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f08a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f08a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="8f08a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08a-119">Request headers</span></span>

| <span data-ttu-id="8f08a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f08a-120">Name</span></span>      |<span data-ttu-id="8f08a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f08a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f08a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f08a-122">Authorization</span></span> | <span data-ttu-id="8f08a-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8f08a-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f08a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08a-124">Request body</span></span>

<span data-ttu-id="8f08a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f08a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f08a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f08a-126">Response</span></span>

<span data-ttu-id="8f08a-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f08a-127">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f08a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f08a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f08a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08a-129">Request</span></span>

<span data-ttu-id="8f08a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f08a-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```

### <a name="response"></a><span data-ttu-id="8f08a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f08a-131">Response</span></span>

<span data-ttu-id="8f08a-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f08a-132">The following is an example of the response.</span></span>

> <span data-ttu-id="8f08a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f08a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->