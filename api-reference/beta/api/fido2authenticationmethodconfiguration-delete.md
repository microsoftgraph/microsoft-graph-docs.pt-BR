---
title: Excluir fido2AuthenticationMethodConfiguration
description: Excluir um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dbb2b7d2c8948763ffc48ac299cc3f2f330498a
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418165"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="dee88-103">Excluir fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="dee88-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="dee88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dee88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dee88-105">Remova as alterações feitas na [política de método de autenticação do FIDO2](../resources/fido2authenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="dee88-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="dee88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dee88-106">Permissions</span></span>
<span data-ttu-id="dee88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dee88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dee88-109">Permission type</span></span>|<span data-ttu-id="dee88-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dee88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dee88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dee88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dee88-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dee88-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="dee88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dee88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dee88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dee88-114">Not supported.</span></span>|
|<span data-ttu-id="dee88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dee88-115">Application</span></span>|<span data-ttu-id="dee88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dee88-116">Not supported.</span></span>|

<span data-ttu-id="dee88-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="dee88-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="dee88-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="dee88-118">Global admin</span></span>
* <span data-ttu-id="dee88-119">Leitor global</span><span class="sxs-lookup"><span data-stu-id="dee88-119">Global reader</span></span>
* <span data-ttu-id="dee88-120">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="dee88-120">Privileged authentication admin</span></span>
* <span data-ttu-id="dee88-121">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="dee88-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="dee88-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dee88-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="dee88-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dee88-123">Request headers</span></span>
|<span data-ttu-id="dee88-124">Nome</span><span class="sxs-lookup"><span data-stu-id="dee88-124">Name</span></span>|<span data-ttu-id="dee88-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="dee88-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dee88-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="dee88-126">Authorization</span></span>|<span data-ttu-id="dee88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dee88-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee88-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dee88-129">Request body</span></span>
<span data-ttu-id="dee88-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dee88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dee88-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dee88-131">Response</span></span>

<span data-ttu-id="dee88-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dee88-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dee88-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dee88-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dee88-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dee88-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="dee88-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dee88-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

