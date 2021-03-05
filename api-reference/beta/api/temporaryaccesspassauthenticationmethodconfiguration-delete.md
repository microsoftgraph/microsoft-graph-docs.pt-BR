---
title: Excluir temporaryAccessPassAuthenticationMethodConfiguration
description: Remova as alterações feitas em um objeto temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 67d2a7ac5e7543e9aff68cf4b9db3a8fef2f2126
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475017"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="5c786-103">Excluir temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c786-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="5c786-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c786-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c786-105">Remova as alterações feitas [no objeto temporaryAccessPassAuthenticationMethodConfiguration revertendo](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="5c786-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c786-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c786-106">Permissions</span></span>
<span data-ttu-id="5c786-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c786-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c786-109">Permission type</span></span>|<span data-ttu-id="5c786-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c786-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c786-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c786-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c786-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c786-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5c786-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c786-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c786-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c786-114">Not supported.</span></span>|
|<span data-ttu-id="5c786-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c786-115">Application</span></span>|<span data-ttu-id="5c786-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c786-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="5c786-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="5c786-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="5c786-118">Para obter mais informações, consulte [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5c786-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5c786-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c786-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="5c786-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c786-120">Request headers</span></span>
|<span data-ttu-id="5c786-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5c786-121">Name</span></span>|<span data-ttu-id="5c786-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c786-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c786-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c786-123">Authorization</span></span>|<span data-ttu-id="5c786-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c786-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c786-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c786-126">Request body</span></span>
<span data-ttu-id="5c786-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c786-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c786-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c786-128">Response</span></span>

<span data-ttu-id="5c786-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c786-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5c786-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c786-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c786-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c786-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5c786-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c786-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
# <a name="c"></a>[<span data-ttu-id="5c786-133">C#</span><span class="sxs-lookup"><span data-stu-id="5c786-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c786-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c786-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c786-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c786-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c786-136">Java</span><span class="sxs-lookup"><span data-stu-id="5c786-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5c786-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c786-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
