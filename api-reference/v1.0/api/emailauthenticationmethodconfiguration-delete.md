---
title: Excluir emailAuthenticationMethodConfiguration
description: Exclui um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 128148d5402d6ddcd2c95bccf17da7d6cbf379bf
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469294"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="c06bb-103">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c06bb-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="c06bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c06bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c06bb-105">Remova as alterações feitas na política de método [de autenticação de email](../resources/emailauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="c06bb-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c06bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c06bb-106">Permissions</span></span>
<span data-ttu-id="c06bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c06bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c06bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c06bb-109">Permission type</span></span>|<span data-ttu-id="c06bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c06bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c06bb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c06bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c06bb-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c06bb-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c06bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c06bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c06bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c06bb-114">Not supported.</span></span>|
|<span data-ttu-id="c06bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c06bb-115">Application</span></span>|<span data-ttu-id="c06bb-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c06bb-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="c06bb-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="c06bb-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="c06bb-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="c06bb-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="c06bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c06bb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="c06bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c06bb-120">Request headers</span></span>

|<span data-ttu-id="c06bb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c06bb-121">Name</span></span>|<span data-ttu-id="c06bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c06bb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c06bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c06bb-123">Authorization</span></span>|<span data-ttu-id="c06bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c06bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c06bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c06bb-126">Request body</span></span>

<span data-ttu-id="c06bb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c06bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c06bb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c06bb-128">Response</span></span>

<span data-ttu-id="c06bb-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c06bb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c06bb-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c06bb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c06bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c06bb-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c06bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c06bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="c06bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="c06bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c06bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c06bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c06bb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c06bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c06bb-136">Java</span><span class="sxs-lookup"><span data-stu-id="c06bb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c06bb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c06bb-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

