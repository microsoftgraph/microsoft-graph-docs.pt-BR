---
title: Excluir emailAuthenticationMethodConfiguration
description: Exclui um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5b9ac408a9de38ceb75f8ee04ee3c442705936d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617105"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="161bf-103">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="161bf-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="161bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="161bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="161bf-105">Remova as alterações feitas na [política de método de autenticação de email](../resources/emailauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="161bf-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="161bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="161bf-106">Permissions</span></span>
<span data-ttu-id="161bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="161bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="161bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="161bf-109">Permission type</span></span>|<span data-ttu-id="161bf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="161bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="161bf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="161bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="161bf-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="161bf-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="161bf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="161bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="161bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="161bf-114">Not supported.</span></span>|
|<span data-ttu-id="161bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="161bf-115">Application</span></span>|<span data-ttu-id="161bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="161bf-116">Not supported.</span></span>|

<span data-ttu-id="161bf-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="161bf-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="161bf-118">Administração global</span><span class="sxs-lookup"><span data-stu-id="161bf-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="161bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="161bf-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="161bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="161bf-120">Request headers</span></span>

|<span data-ttu-id="161bf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="161bf-121">Name</span></span>|<span data-ttu-id="161bf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="161bf-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="161bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="161bf-123">Authorization</span></span>|<span data-ttu-id="161bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="161bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="161bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="161bf-126">Request body</span></span>

<span data-ttu-id="161bf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="161bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="161bf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="161bf-128">Response</span></span>

<span data-ttu-id="161bf-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="161bf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="161bf-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="161bf-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="161bf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="161bf-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="161bf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="161bf-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

