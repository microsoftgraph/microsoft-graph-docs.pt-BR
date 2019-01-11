---
title: Obter identityProvider
description: Recupere as propriedades de um identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: f0d467bde092f84d092dbcee7c54c01e3ef849f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812968"
---
# <a name="get-identityprovider"></a><span data-ttu-id="45488-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="45488-103">Get identityProvider</span></span>

> <span data-ttu-id="45488-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45488-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45488-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45488-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45488-106">Recupere as propriedades de um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="45488-106">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45488-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="45488-107">Permissions</span></span>

<span data-ttu-id="45488-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45488-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45488-110">Permission type</span></span>      | <span data-ttu-id="45488-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45488-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45488-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45488-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45488-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45488-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="45488-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45488-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="45488-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45488-115">Not supported.</span></span>|
|<span data-ttu-id="45488-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45488-116">Application</span></span>|<span data-ttu-id="45488-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45488-117">Not supported.</span></span>|

<span data-ttu-id="45488-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="45488-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="45488-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45488-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45488-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45488-120">Request headers</span></span>

|<span data-ttu-id="45488-121">Nome</span><span class="sxs-lookup"><span data-stu-id="45488-121">Name</span></span>|<span data-ttu-id="45488-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="45488-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="45488-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45488-123">Authorization</span></span>|<span data-ttu-id="45488-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45488-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45488-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45488-126">Request body</span></span>

<span data-ttu-id="45488-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45488-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45488-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="45488-128">Response</span></span>

<span data-ttu-id="45488-129">Se tiver êxito, este método retornará `200 OK` código de resposta e uma representação de JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45488-129">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45488-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45488-130">Example</span></span>

<span data-ttu-id="45488-131">O exemplo a seguir recupera um específicos **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="45488-131">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="45488-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45488-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="45488-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="45488-133">Response</span></span>

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
