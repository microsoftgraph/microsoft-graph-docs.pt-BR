---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c1090c2ab71e66779d643e5149b3a053d35f5a7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458819"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="d225d-103">Obter fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d225d-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="d225d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d225d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d225d-105">Recupere as propriedades e os relacionamentos do objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , que representa a [política de método de autenticação](../resources/authenticationmethodspolicies-overview.md) de chaves de segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d225d-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d225d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d225d-106">Permissions</span></span>
<span data-ttu-id="d225d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d225d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d225d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d225d-109">Permission type</span></span>|<span data-ttu-id="d225d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d225d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d225d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d225d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d225d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d225d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d225d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d225d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d225d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d225d-114">Not supported.</span></span>|
|<span data-ttu-id="d225d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d225d-115">Application</span></span>|<span data-ttu-id="d225d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d225d-116">Not supported.</span></span>|

<span data-ttu-id="d225d-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="d225d-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d225d-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d225d-118">Global admin</span></span>
* <span data-ttu-id="d225d-119">Leitor global</span><span class="sxs-lookup"><span data-stu-id="d225d-119">Global reader</span></span>
* <span data-ttu-id="d225d-120">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d225d-120">Privileged authentication admin</span></span>
* <span data-ttu-id="d225d-121">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="d225d-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d225d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d225d-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="d225d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d225d-123">Request headers</span></span>
|<span data-ttu-id="d225d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d225d-124">Name</span></span>|<span data-ttu-id="d225d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d225d-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d225d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d225d-126">Authorization</span></span>|<span data-ttu-id="d225d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d225d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d225d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d225d-129">Request body</span></span>
<span data-ttu-id="d225d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d225d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d225d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d225d-131">Response</span></span>

<span data-ttu-id="d225d-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d225d-132">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d225d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d225d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d225d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d225d-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="d225d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d225d-135">Response</span></span>
<span data-ttu-id="d225d-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d225d-136">The following is an example of the response.</span></span>

<span data-ttu-id="d225d-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d225d-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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

