---
title: Obter phoneAuthenticationMethod
description: Recupere um único objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0eee3702c31c5237d8b1f322018dcc60bc63762c
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557784"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="b7260-103">Obter phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b7260-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="b7260-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7260-105">Recupere um único objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="b7260-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7260-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7260-106">Permissions</span></span>

<span data-ttu-id="b7260-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7260-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7260-109">Permission type</span></span>                        | <span data-ttu-id="b7260-110">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7260-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="b7260-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7260-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b7260-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7260-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7260-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7260-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="b7260-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7260-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b7260-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7260-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7260-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7260-116">Not supported.</span></span> | <span data-ttu-id="b7260-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7260-117">Not supported.</span></span> |
| <span data-ttu-id="b7260-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7260-118">Application</span></span>                            | <span data-ttu-id="b7260-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7260-119">Not supported.</span></span> | <span data-ttu-id="b7260-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7260-120">Not supported.</span></span> |

<span data-ttu-id="b7260-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="b7260-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b7260-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b7260-122">Global admin</span></span>
* <span data-ttu-id="b7260-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="b7260-123">Global reader</span></span>
* <span data-ttu-id="b7260-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b7260-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b7260-125">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="b7260-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b7260-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7260-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7260-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7260-127">Optional query parameters</span></span>

<span data-ttu-id="b7260-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7260-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7260-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7260-129">Request headers</span></span>

| <span data-ttu-id="b7260-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b7260-130">Name</span></span>      |<span data-ttu-id="b7260-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7260-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7260-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7260-132">Authorization</span></span> | <span data-ttu-id="b7260-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7260-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7260-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7260-135">Request body</span></span>

<span data-ttu-id="b7260-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7260-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7260-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7260-137">Response</span></span>

<span data-ttu-id="b7260-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7260-138">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7260-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7260-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7260-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7260-140">Request</span></span>

<span data-ttu-id="b7260-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7260-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```http
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```

### <a name="response"></a><span data-ttu-id="b7260-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7260-142">Response</span></span>

<span data-ttu-id="b7260-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7260-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b7260-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7260-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
