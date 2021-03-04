---
title: Excluir microsoftAuthenticatorAuthenticationMethodConfiguration
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 132ad08227887d13bdf9b11b413dfb711acb9a2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447842"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="81483-103">Excluir microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="81483-103">Delete microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="81483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81483-105">Remova as alterações feitas na política de método de autenticação [do Microsoft Authenticator](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="81483-105">Remove changes made to the [Microsoft Authenticator authentication method policy](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="81483-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81483-106">Permissions</span></span>
<span data-ttu-id="81483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81483-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81483-109">Permission type</span></span>|<span data-ttu-id="81483-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81483-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81483-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81483-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81483-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81483-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="81483-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81483-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81483-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81483-114">Not supported.</span></span>|
|<span data-ttu-id="81483-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81483-115">Application</span></span>|<span data-ttu-id="81483-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81483-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="81483-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="81483-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="81483-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="81483-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="81483-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81483-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="81483-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81483-120">Request headers</span></span>
|<span data-ttu-id="81483-121">Nome</span><span class="sxs-lookup"><span data-stu-id="81483-121">Name</span></span>|<span data-ttu-id="81483-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81483-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81483-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81483-123">Authorization</span></span>|<span data-ttu-id="81483-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81483-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81483-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81483-126">Request body</span></span>
<span data-ttu-id="81483-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81483-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81483-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81483-128">Response</span></span>

<span data-ttu-id="81483-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81483-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="81483-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81483-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81483-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81483-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="81483-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="81483-132">Response</span></span>
<span data-ttu-id="81483-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81483-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

