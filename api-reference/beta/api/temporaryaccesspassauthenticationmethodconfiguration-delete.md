---
title: Excluir temporaryAccessPassAuthenticationMethodConfiguration
description: Remover alterações feitas em um objeto temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37ea21542aa9ceace151428fcf951c0a87ecbf82
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272597"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="22ae3-103">Excluir temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="22ae3-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="22ae3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ae3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ae3-105">Remova as alterações feitas no [objeto temporaryAccessPassAuthenticationMethodConfiguration revertendo](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="22ae3-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="22ae3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="22ae3-106">Permissions</span></span>
<span data-ttu-id="22ae3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ae3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22ae3-109">Permission type</span></span>|<span data-ttu-id="22ae3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22ae3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ae3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22ae3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22ae3-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22ae3-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="22ae3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22ae3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ae3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ae3-114">Not supported.</span></span>|
|<span data-ttu-id="22ae3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22ae3-115">Application</span></span>|<span data-ttu-id="22ae3-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22ae3-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="22ae3-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="22ae3-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="22ae3-118">Para obter mais informações, consulte [funções.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="22ae3-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="22ae3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22ae3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="22ae3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22ae3-120">Request headers</span></span>
|<span data-ttu-id="22ae3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22ae3-121">Name</span></span>|<span data-ttu-id="22ae3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22ae3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22ae3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22ae3-123">Authorization</span></span>|<span data-ttu-id="22ae3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22ae3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ae3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22ae3-126">Request body</span></span>
<span data-ttu-id="22ae3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22ae3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22ae3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ae3-128">Response</span></span>

<span data-ttu-id="22ae3-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22ae3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="22ae3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22ae3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22ae3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22ae3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


### <a name="response"></a><span data-ttu-id="22ae3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ae3-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
