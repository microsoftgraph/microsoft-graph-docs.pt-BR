---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f1420ffc51305777e3b40710cfb85893f7c4b2e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202594"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="b45bb-103">Obter fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b45bb-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="b45bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b45bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b45bb-105">Recupere as propriedades e as relações do objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) [](../resources/authenticationmethodspolicies-overview.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b45bb-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b45bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b45bb-106">Permissions</span></span>
<span data-ttu-id="b45bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b45bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b45bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b45bb-109">Permission type</span></span>|<span data-ttu-id="b45bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b45bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b45bb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b45bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b45bb-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b45bb-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="b45bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b45bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b45bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b45bb-114">Not supported.</span></span>|
|<span data-ttu-id="b45bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b45bb-115">Application</span></span>|<span data-ttu-id="b45bb-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b45bb-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="b45bb-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="b45bb-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="b45bb-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="b45bb-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="b45bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b45bb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="b45bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b45bb-120">Request headers</span></span>
|<span data-ttu-id="b45bb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b45bb-121">Name</span></span>|<span data-ttu-id="b45bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b45bb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b45bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b45bb-123">Authorization</span></span>|<span data-ttu-id="b45bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b45bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b45bb-126">Request body</span></span>
<span data-ttu-id="b45bb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b45bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b45bb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b45bb-128">Response</span></span>

<span data-ttu-id="b45bb-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b45bb-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b45bb-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b45bb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b45bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b45bb-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b45bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b45bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="b45bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="b45bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b45bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b45bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b45bb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b45bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b45bb-136">Java</span><span class="sxs-lookup"><span data-stu-id="b45bb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b45bb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b45bb-137">Response</span></span>
<span data-ttu-id="b45bb-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b45bb-138">The following is an example of the response.</span></span>

<span data-ttu-id="b45bb-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b45bb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "value":{
      "@odata.type":"#microsoft.graph.fido2AuthenticationMethodConfiguration",
      "id":"Fido2",
      "state":"enabled",
      "isSelfServiceRegistrationAllowed":true,
      "isAttestationEnforced":true,
      "keyRestrictions":{
         "isEnforced":false,
         "enforcementType":"block",
         "aaGuids":[
            
         ]
      },
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false,
            "useForSignIn":true
         }
      ]
   }
}
```

