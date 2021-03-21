---
title: Excluir fido2AuthenticationMethodConfiguration
description: Exclua um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dbf6514a7dc21cb078f369d5e1e1db66f374661
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964633"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="4dfa6-103">Excluir fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4dfa6-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4dfa6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dfa6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4dfa6-105">Remova as alterações feitas na política de método de autenticação [FIDO2](../resources/fido2authenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dfa6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dfa6-106">Permissions</span></span>
<span data-ttu-id="4dfa6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dfa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4dfa6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dfa6-109">Permission type</span></span>|<span data-ttu-id="4dfa6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dfa6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dfa6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dfa6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4dfa6-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4dfa6-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4dfa6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dfa6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dfa6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-114">Not supported.</span></span>|
|<span data-ttu-id="4dfa6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dfa6-115">Application</span></span>|<span data-ttu-id="4dfa6-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4dfa6-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="4dfa6-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="4dfa6-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="4dfa6-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="4dfa6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dfa6-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="4dfa6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfa6-120">Request headers</span></span>
|<span data-ttu-id="4dfa6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4dfa6-121">Name</span></span>|<span data-ttu-id="4dfa6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfa6-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4dfa6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dfa6-123">Authorization</span></span>|<span data-ttu-id="4dfa6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dfa6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfa6-126">Request body</span></span>
<span data-ttu-id="4dfa6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dfa6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfa6-128">Response</span></span>

<span data-ttu-id="4dfa6-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4dfa6-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4dfa6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4dfa6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4dfa6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfa6-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="4dfa6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfa6-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

