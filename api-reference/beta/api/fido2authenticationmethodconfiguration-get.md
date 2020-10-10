---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5411f9c76b6870eccdb43863b5a62380d7caafa3
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418169"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="1ea69-103">Obter fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ea69-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1ea69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ea69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ea69-105">Recupere as propriedades e os relacionamentos do objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , que representa a [política de método de autenticação](../resources/authenticationmethodspolicies-overview.md) de chaves de segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1ea69-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ea69-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ea69-106">Permissions</span></span>
<span data-ttu-id="1ea69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ea69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ea69-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ea69-109">Permission type</span></span>|<span data-ttu-id="1ea69-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ea69-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ea69-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ea69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ea69-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ea69-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1ea69-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ea69-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ea69-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ea69-114">Not supported.</span></span>|
|<span data-ttu-id="1ea69-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ea69-115">Application</span></span>|<span data-ttu-id="1ea69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ea69-116">Not supported.</span></span>|

<span data-ttu-id="1ea69-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1ea69-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1ea69-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1ea69-118">Global admin</span></span>
* <span data-ttu-id="1ea69-119">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1ea69-119">Global reader</span></span>
* <span data-ttu-id="1ea69-120">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1ea69-120">Privileged authentication admin</span></span>
* <span data-ttu-id="1ea69-121">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="1ea69-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1ea69-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ea69-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="1ea69-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea69-123">Request headers</span></span>
|<span data-ttu-id="1ea69-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1ea69-124">Name</span></span>|<span data-ttu-id="1ea69-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea69-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1ea69-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ea69-126">Authorization</span></span>|<span data-ttu-id="1ea69-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ea69-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ea69-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea69-129">Request body</span></span>
<span data-ttu-id="1ea69-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ea69-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ea69-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea69-131">Response</span></span>

<span data-ttu-id="1ea69-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ea69-132">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ea69-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1ea69-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ea69-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea69-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="1ea69-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea69-135">Response</span></span>
<span data-ttu-id="1ea69-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1ea69-136">The following is an example of the response.</span></span>

<span data-ttu-id="1ea69-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1ea69-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "id": "Fido2",
    "state": "enabled",
    "isSelfServiceRegistrationAllowed": true,
    "isAttestationEnforced": true,
    "keyRestrictions": {
        "isEnforced": false,
        "enforcementType": "block",
        "aaGuids": []
    },
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
  }
}
```

