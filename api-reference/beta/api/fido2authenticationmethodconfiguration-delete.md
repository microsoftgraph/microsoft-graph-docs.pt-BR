---
title: Excluir fido2AuthenticationMethodConfiguration
description: Exclua um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 473c0605cc302b29730ddb359f51904050296ff2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873000"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="a9c5a-103">Excluir fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9c5a-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="a9c5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9c5a-105">Remova as alterações feitas na política de método de autenticação [FIDO2](../resources/fido2authenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9c5a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9c5a-106">Permissions</span></span>
<span data-ttu-id="a9c5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9c5a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9c5a-109">Permission type</span></span>|<span data-ttu-id="a9c5a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9c5a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9c5a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9c5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9c5a-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a9c5a-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="a9c5a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9c5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9c5a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-114">Not supported.</span></span>|
|<span data-ttu-id="a9c5a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9c5a-115">Application</span></span>|<span data-ttu-id="a9c5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-116">Not supported.</span></span>|

<span data-ttu-id="a9c5a-117">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a9c5a-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="a9c5a-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a9c5a-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="a9c5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9c5a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="a9c5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5a-120">Request headers</span></span>
|<span data-ttu-id="a9c5a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a9c5a-121">Name</span></span>|<span data-ttu-id="a9c5a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c5a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9c5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9c5a-123">Authorization</span></span>|<span data-ttu-id="a9c5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c5a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5a-126">Request body</span></span>
<span data-ttu-id="a9c5a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9c5a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c5a-128">Response</span></span>

<span data-ttu-id="a9c5a-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9c5a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a9c5a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9c5a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9c5a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="a9c5a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c5a-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

