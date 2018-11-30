---
title: Lista identityProviders
description: Recupere todos os identityProviders no diretório.
ms.openlocfilehash: fd5662690b644bc7a34587a5bdfc519188a3d4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039285"
---
# <a name="list-identityproviders"></a><span data-ttu-id="d9a63-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="d9a63-103">List identityProviders</span></span>

> <span data-ttu-id="d9a63-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9a63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9a63-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9a63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9a63-106">Recupere todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="d9a63-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9a63-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9a63-107">Permissions</span></span>

<span data-ttu-id="d9a63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9a63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a63-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9a63-110">Permission type</span></span>      | <span data-ttu-id="d9a63-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9a63-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9a63-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9a63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9a63-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a63-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d9a63-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9a63-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d9a63-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a63-115">Not supported.</span></span>|
|<span data-ttu-id="d9a63-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9a63-116">Application</span></span>|<span data-ttu-id="d9a63-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a63-117">Not supported.</span></span>|

<span data-ttu-id="d9a63-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="d9a63-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9a63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a63-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="d9a63-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a63-120">Request headers</span></span>

|<span data-ttu-id="d9a63-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d9a63-121">Name</span></span>|<span data-ttu-id="d9a63-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9a63-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d9a63-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9a63-123">Authorization</span></span>|<span data-ttu-id="d9a63-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9a63-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9a63-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a63-126">Request body</span></span>

<span data-ttu-id="d9a63-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9a63-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9a63-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a63-128">Response</span></span>

<span data-ttu-id="d9a63-129">Se tiver êxito, este método retornará `200 OK` código de resposta e uma coleção de [identityProviders](../resources/identityprovider.md) na representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a63-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9a63-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9a63-130">Example</span></span>

<span data-ttu-id="d9a63-131">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="d9a63-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d9a63-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a63-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="d9a63-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a63-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->