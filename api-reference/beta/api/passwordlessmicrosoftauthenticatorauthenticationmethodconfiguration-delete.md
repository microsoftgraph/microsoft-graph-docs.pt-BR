---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Excluir um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eafbb6940a3d70e7191c18369e2764c137f0d674
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086638"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="3a9b6-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a9b6-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="3a9b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a9b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a9b6-105">Remova as alterações feitas na [política de método de autenticação de entrada de telefone do Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="3a9b6-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="3a9b6-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a9b6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a9b6-108">Permissions</span></span>
<span data-ttu-id="3a9b6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a9b6-111">Permission type</span></span>|<span data-ttu-id="3a9b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a9b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9b6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a9b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9b6-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3a9b6-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="3a9b6-115">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="3a9b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-116">Not supported.</span></span>|
|<span data-ttu-id="3a9b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a9b6-117">Application</span></span>|<span data-ttu-id="3a9b6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-118">Not supported.</span></span>|

<span data-ttu-id="3a9b6-119">Para cenários delegados, o administrador precisa da seguinte [função](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="3a9b6-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="3a9b6-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3a9b6-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="3a9b6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9b6-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="3a9b6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9b6-122">Request headers</span></span>
|<span data-ttu-id="3a9b6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3a9b6-123">Name</span></span>|<span data-ttu-id="3a9b6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a9b6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a9b6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a9b6-125">Authorization</span></span>|<span data-ttu-id="3a9b6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9b6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9b6-128">Request body</span></span>
<span data-ttu-id="3a9b6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a9b6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9b6-130">Response</span></span>

<span data-ttu-id="3a9b6-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a9b6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3a9b6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a9b6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a9b6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9b6-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="3a9b6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9b6-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

