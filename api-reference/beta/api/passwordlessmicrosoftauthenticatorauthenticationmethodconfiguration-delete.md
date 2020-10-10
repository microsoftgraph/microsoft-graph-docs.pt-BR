---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Excluir um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3200e95acdee4042c3933d5926662d6e49d52052
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418218"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="82cc6-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="82cc6-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="82cc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82cc6-105">Remova as alterações feitas na [política de método de autenticação de entrada de telefone do Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="82cc6-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="82cc6-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="82cc6-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="82cc6-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="82cc6-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="82cc6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="82cc6-108">Permissions</span></span>
<span data-ttu-id="82cc6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cc6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82cc6-111">Permission type</span></span>|<span data-ttu-id="82cc6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82cc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82cc6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82cc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82cc6-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="82cc6-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="82cc6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82cc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82cc6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82cc6-116">Not supported.</span></span>|
|<span data-ttu-id="82cc6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82cc6-117">Application</span></span>|<span data-ttu-id="82cc6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82cc6-118">Not supported.</span></span>|

<span data-ttu-id="82cc6-119">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="82cc6-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="82cc6-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="82cc6-120">Global admin</span></span>
* <span data-ttu-id="82cc6-121">Leitor global</span><span class="sxs-lookup"><span data-stu-id="82cc6-121">Global reader</span></span>
* <span data-ttu-id="82cc6-122">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="82cc6-122">Privileged authentication admin</span></span>
* <span data-ttu-id="82cc6-123">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="82cc6-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="82cc6-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82cc6-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="82cc6-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc6-125">Request headers</span></span>
|<span data-ttu-id="82cc6-126">Nome</span><span class="sxs-lookup"><span data-stu-id="82cc6-126">Name</span></span>|<span data-ttu-id="82cc6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="82cc6-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82cc6-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="82cc6-128">Authorization</span></span>|<span data-ttu-id="82cc6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82cc6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82cc6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc6-131">Request body</span></span>
<span data-ttu-id="82cc6-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82cc6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82cc6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cc6-133">Response</span></span>

<span data-ttu-id="82cc6-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82cc6-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="82cc6-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="82cc6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82cc6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc6-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="82cc6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cc6-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

