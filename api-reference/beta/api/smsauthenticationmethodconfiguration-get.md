---
title: Obter smsAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc09a85fefb46142c46d5383a0d7225636041b8b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761846"
---
# <a name="get-smsauthenticationmethodconfiguration"></a><span data-ttu-id="3cd1e-103">Obter smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cd1e-103">Get smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="3cd1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd1e-105">Leia as propriedades e as relações de um [objeto smsAuthenticationMethodConfiguration,](../resources/smsauthenticationmethodconfiguration.md) que representa a política de método de autenticação de Mensagem de Texto para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-105">Read the properties and relationships of a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object, which represents the Text Message authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cd1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd1e-106">Permissions</span></span>
<span data-ttu-id="3cd1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd1e-109">Permission type</span></span>|<span data-ttu-id="3cd1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cd1e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd1e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd1e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd1e-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3cd1e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="3cd1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd1e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-114">Not supported.</span></span>|
|<span data-ttu-id="3cd1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd1e-115">Application</span></span>|<span data-ttu-id="3cd1e-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3cd1e-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="3cd1e-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="3cd1e-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="3cd1e-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="3cd1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd1e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="3cd1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd1e-120">Request headers</span></span>
|<span data-ttu-id="3cd1e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3cd1e-121">Name</span></span>|<span data-ttu-id="3cd1e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd1e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cd1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd1e-123">Authorization</span></span>|<span data-ttu-id="3cd1e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd1e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd1e-126">Request body</span></span>
<span data-ttu-id="3cd1e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cd1e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd1e-128">Response</span></span>

<span data-ttu-id="3cd1e-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-129">If successful, this method returns a `200 OK` response code and a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cd1e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3cd1e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cd1e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd1e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3cd1e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd1e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_smsauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```
# <a name="c"></a>[<span data-ttu-id="3cd1e-133">C#</span><span class="sxs-lookup"><span data-stu-id="3cd1e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cd1e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cd1e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cd1e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cd1e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cd1e-136">Java</span><span class="sxs-lookup"><span data-stu-id="3cd1e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cd1e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd1e-137">Response</span></span>
<span data-ttu-id="3cd1e-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3cd1e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "713980c7-80c7-7139-c780-3971c7803971",
    "state": "String"
  }
}
```

