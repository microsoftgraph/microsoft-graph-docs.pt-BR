---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c394bf0d75e9115f3cfe7ec44ff4978f716401d0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435989"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="f7e68-103">Obter fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7e68-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="f7e68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7e68-105">Recupere as propriedades e as relações do objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) [](../resources/authenticationmethodspolicies-overview.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f7e68-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7e68-106">Permissions</span></span>
<span data-ttu-id="f7e68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7e68-109">Permission type</span></span>|<span data-ttu-id="f7e68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7e68-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e68-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7e68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7e68-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f7e68-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="f7e68-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7e68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e68-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7e68-114">Not supported.</span></span>|
|<span data-ttu-id="f7e68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7e68-115">Application</span></span>|<span data-ttu-id="f7e68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7e68-116">Not supported.</span></span>|

<span data-ttu-id="f7e68-117">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f7e68-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="f7e68-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f7e68-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="f7e68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e68-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="f7e68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e68-120">Request headers</span></span>
|<span data-ttu-id="f7e68-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f7e68-121">Name</span></span>|<span data-ttu-id="f7e68-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7e68-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7e68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7e68-123">Authorization</span></span>|<span data-ttu-id="f7e68-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7e68-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e68-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e68-126">Request body</span></span>
<span data-ttu-id="f7e68-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7e68-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e68-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7e68-128">Response</span></span>

<span data-ttu-id="f7e68-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7e68-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7e68-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7e68-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7e68-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e68-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="f7e68-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7e68-132">Response</span></span>
<span data-ttu-id="f7e68-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7e68-133">The following is an example of the response.</span></span>

<span data-ttu-id="f7e68-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7e68-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

