---
title: Excluir microsoftAuthenticatorAuthenticationMethodConfiguration
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93a16ae2865fcdb85963c7e8aded8e5ca6727720
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202734"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="71dfc-103">Excluir microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="71dfc-103">Delete microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="71dfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71dfc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71dfc-105">Remova as alterações feitas na política de método de autenticação [do Microsoft Authenticator](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="71dfc-105">Remove changes made to the [Microsoft Authenticator authentication method policy](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="71dfc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71dfc-106">Permissions</span></span>
<span data-ttu-id="71dfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71dfc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71dfc-109">Permission type</span></span>|<span data-ttu-id="71dfc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71dfc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71dfc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71dfc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71dfc-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="71dfc-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="71dfc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71dfc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71dfc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71dfc-114">Not supported.</span></span>|
|<span data-ttu-id="71dfc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71dfc-115">Application</span></span>|<span data-ttu-id="71dfc-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="71dfc-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="71dfc-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="71dfc-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="71dfc-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="71dfc-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="71dfc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71dfc-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="71dfc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfc-120">Request headers</span></span>
|<span data-ttu-id="71dfc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="71dfc-121">Name</span></span>|<span data-ttu-id="71dfc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71dfc-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71dfc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71dfc-123">Authorization</span></span>|<span data-ttu-id="71dfc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71dfc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71dfc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfc-126">Request body</span></span>
<span data-ttu-id="71dfc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71dfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71dfc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dfc-128">Response</span></span>

<span data-ttu-id="71dfc-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71dfc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="71dfc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71dfc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71dfc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71dfc-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="71dfc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="71dfc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="71dfc-133">C#</span><span class="sxs-lookup"><span data-stu-id="71dfc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71dfc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71dfc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71dfc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71dfc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71dfc-136">Java</span><span class="sxs-lookup"><span data-stu-id="71dfc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="71dfc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dfc-137">Response</span></span>
<span data-ttu-id="71dfc-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="71dfc-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

