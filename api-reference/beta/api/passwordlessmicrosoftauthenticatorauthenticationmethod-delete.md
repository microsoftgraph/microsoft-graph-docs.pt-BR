---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Exclui um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f5b91f65326fd14fe648b9a94c54a8e0db1920f
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418220"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="784ed-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="784ed-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="784ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="784ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="784ed-105">Exclui o objeto de [método de entrada de telefone sem senha do autenticador da Microsoft](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="784ed-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="784ed-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="784ed-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="784ed-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="784ed-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="784ed-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="784ed-108">Permissions</span></span>
<span data-ttu-id="784ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="784ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="784ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="784ed-111">Permission type</span></span>|<span data-ttu-id="784ed-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="784ed-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="784ed-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="784ed-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="784ed-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="784ed-114">Delegated (work or school account)</span></span>|<span data-ttu-id="784ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784ed-115">Not supported.</span></span>|<span data-ttu-id="784ed-116">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="784ed-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="784ed-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="784ed-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="784ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784ed-118">Not supported.</span></span>|<span data-ttu-id="784ed-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784ed-119">Not supported.</span></span>
|<span data-ttu-id="784ed-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="784ed-120">Application</span></span>|<span data-ttu-id="784ed-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784ed-121">Not supported.</span></span>|<span data-ttu-id="784ed-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784ed-122">Not supported.</span></span>

<span data-ttu-id="784ed-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="784ed-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="784ed-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="784ed-124">Global admin</span></span>
* <span data-ttu-id="784ed-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="784ed-125">Global reader</span></span>
* <span data-ttu-id="784ed-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="784ed-126">Privileged authentication admin</span></span>
* <span data-ttu-id="784ed-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="784ed-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="784ed-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="784ed-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="784ed-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="784ed-129">Request headers</span></span>
|<span data-ttu-id="784ed-130">Nome</span><span class="sxs-lookup"><span data-stu-id="784ed-130">Name</span></span>|<span data-ttu-id="784ed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="784ed-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="784ed-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="784ed-132">Authorization</span></span>|<span data-ttu-id="784ed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="784ed-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="784ed-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="784ed-135">Request body</span></span>
<span data-ttu-id="784ed-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="784ed-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="784ed-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="784ed-137">Response</span></span>

<span data-ttu-id="784ed-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="784ed-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="784ed-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="784ed-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="784ed-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="784ed-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```


### <a name="response"></a><span data-ttu-id="784ed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="784ed-142">Response</span></span>
<span data-ttu-id="784ed-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="784ed-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

