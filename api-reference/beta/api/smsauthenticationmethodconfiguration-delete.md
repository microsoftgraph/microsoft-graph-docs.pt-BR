---
title: Excluir smsAuthenticationMethodConfiguration
description: Exclua um objeto smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec22cabd9ca43a6415509f114fa1592855f0b8a8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475615"
---
# <a name="delete-smsauthenticationmethodconfiguration"></a><span data-ttu-id="a3cb2-103">Excluir smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3cb2-103">Delete smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="a3cb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3cb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3cb2-105">Remova as alterações feitas na política de método de [autenticação](../resources/smsauthenticationmethodconfiguration.md) de Mensagem de Texto revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-105">Remove changes made to the [Text Message authentication method policy](../resources/smsauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3cb2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3cb2-106">Permissions</span></span>
<span data-ttu-id="a3cb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3cb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3cb2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3cb2-109">Permission type</span></span>|<span data-ttu-id="a3cb2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3cb2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3cb2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3cb2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3cb2-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a3cb2-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="a3cb2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3cb2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3cb2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-114">Not supported.</span></span>|
|<span data-ttu-id="a3cb2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3cb2-115">Application</span></span>|<span data-ttu-id="a3cb2-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a3cb2-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="a3cb2-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="a3cb2-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="a3cb2-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="a3cb2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3cb2-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="a3cb2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3cb2-120">Request headers</span></span>
|<span data-ttu-id="a3cb2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a3cb2-121">Name</span></span>|<span data-ttu-id="a3cb2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3cb2-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3cb2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3cb2-123">Authorization</span></span>|<span data-ttu-id="a3cb2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3cb2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3cb2-126">Request body</span></span>
<span data-ttu-id="a3cb2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3cb2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3cb2-128">Response</span></span>

<span data-ttu-id="a3cb2-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a3cb2-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3cb2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3cb2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3cb2-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a3cb2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3cb2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_smsauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```
# <a name="c"></a>[<span data-ttu-id="a3cb2-133">C#</span><span class="sxs-lookup"><span data-stu-id="a3cb2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3cb2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3cb2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3cb2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3cb2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3cb2-136">Java</span><span class="sxs-lookup"><span data-stu-id="a3cb2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a3cb2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3cb2-137">Response</span></span>
<span data-ttu-id="a3cb2-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3cb2-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

