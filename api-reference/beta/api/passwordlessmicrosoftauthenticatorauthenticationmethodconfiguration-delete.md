---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Exclua um objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7b7cb8cc0eca09dde9e4ecb56a570bf1faf92b05
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873448"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="5a0ff-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (preterido)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="5a0ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a0ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a0ff-105">Remova as alterações feitas na política de método de autenticação de Entrada de Telefone do [Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!CAUTION]
> <span data-ttu-id="5a0ff-106">A API do método de autenticação de autenticação de telefone sem senha do Microsoft Authenticator foi preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="5a0ff-107">Use a nova política [de método de autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a0ff-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a0ff-108">Permissions</span></span>
<span data-ttu-id="5a0ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a0ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a0ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a0ff-111">Permission type</span></span>|<span data-ttu-id="5a0ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a0ff-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a0ff-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5a0ff-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5a0ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a0ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-116">Not supported.</span></span>|
|<span data-ttu-id="5a0ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a0ff-117">Application</span></span>|<span data-ttu-id="5a0ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-118">Not supported.</span></span>|

<span data-ttu-id="5a0ff-119">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5a0ff-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5a0ff-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5a0ff-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="5a0ff-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a0ff-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="5a0ff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a0ff-122">Request headers</span></span>
|<span data-ttu-id="5a0ff-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5a0ff-123">Name</span></span>|<span data-ttu-id="5a0ff-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a0ff-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a0ff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a0ff-125">Authorization</span></span>|<span data-ttu-id="5a0ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a0ff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a0ff-128">Request body</span></span>
<span data-ttu-id="5a0ff-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a0ff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a0ff-130">Response</span></span>

<span data-ttu-id="5a0ff-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5a0ff-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a0ff-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a0ff-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a0ff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a0ff-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="5a0ff-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a0ff-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

