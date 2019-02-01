---
title: Obter identityProvider
description: Recuperar as propriedades de um identityProvider existente
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc06d4f8dcab8bf07d2dc0a9ff8130b305b8217c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649355"
---
# <a name="get-identityprovider"></a><span data-ttu-id="6a3a3-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="6a3a3-103">Get identityProvider</span></span>

<span data-ttu-id="6a3a3-104">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a3a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a3a3-105">Permissions</span></span>

<span data-ttu-id="6a3a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a3a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a3a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a3a3-108">Permission type</span></span>      | <span data-ttu-id="6a3a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a3a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a3a3-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a3a3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6a3a3-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a3a3-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6a3a3-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a3a3-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6a3a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-113">Not supported.</span></span>|
|<span data-ttu-id="6a3a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a3a3-114">Application</span></span>|<span data-ttu-id="6a3a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-115">Not supported.</span></span>|

<span data-ttu-id="6a3a3-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a3a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a3a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a3a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a3a3-118">Request headers</span></span>

|<span data-ttu-id="6a3a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6a3a3-119">Name</span></span>|<span data-ttu-id="6a3a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3a3-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6a3a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a3a3-121">Authorization</span></span>|<span data-ttu-id="6a3a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a3a3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a3a3-124">Request body</span></span>

<span data-ttu-id="6a3a3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a3a3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a3a3-126">Response</span></span>

<span data-ttu-id="6a3a3-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityProvider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-127">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/identityProvider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a3a3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a3a3-128">Example</span></span>

<span data-ttu-id="6a3a3-129">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="6a3a3-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="6a3a3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a3a3-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="6a3a3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a3a3-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
