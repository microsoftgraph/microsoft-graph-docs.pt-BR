---
title: Excluir emailAuthenticationMethodConfiguration
description: Exclui um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b25e0545eba722ab251a450600eb587d2ebad35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964575"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="d221e-103">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d221e-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="d221e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d221e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d221e-105">Remova as alterações feitas na política de método [de autenticação de email](../resources/emailauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="d221e-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d221e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d221e-106">Permissions</span></span>
<span data-ttu-id="d221e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d221e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d221e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d221e-109">Permission type</span></span>|<span data-ttu-id="d221e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d221e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d221e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d221e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d221e-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d221e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d221e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d221e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d221e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d221e-114">Not supported.</span></span>|
|<span data-ttu-id="d221e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d221e-115">Application</span></span>|<span data-ttu-id="d221e-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d221e-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="d221e-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="d221e-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="d221e-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="d221e-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="d221e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d221e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="d221e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d221e-120">Request headers</span></span>

|<span data-ttu-id="d221e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d221e-121">Name</span></span>|<span data-ttu-id="d221e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d221e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d221e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d221e-123">Authorization</span></span>|<span data-ttu-id="d221e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d221e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d221e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d221e-126">Request body</span></span>

<span data-ttu-id="d221e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d221e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d221e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d221e-128">Response</span></span>

<span data-ttu-id="d221e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d221e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d221e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d221e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d221e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d221e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="d221e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d221e-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

