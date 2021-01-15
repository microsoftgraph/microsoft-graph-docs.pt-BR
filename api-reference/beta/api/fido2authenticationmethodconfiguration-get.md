---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 19e751bab6f076f7269ca895abc35f40a1160423
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872993"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="1cf82-103">Obter fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cf82-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1cf82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cf82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cf82-105">Recupere as propriedades e as relações do objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) [](../resources/authenticationmethodspolicies-overview.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1cf82-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cf82-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cf82-106">Permissions</span></span>
<span data-ttu-id="1cf82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cf82-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cf82-109">Permission type</span></span>|<span data-ttu-id="1cf82-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cf82-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cf82-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cf82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cf82-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1cf82-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1cf82-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cf82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cf82-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cf82-114">Not supported.</span></span>|
|<span data-ttu-id="1cf82-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cf82-115">Application</span></span>|<span data-ttu-id="1cf82-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cf82-116">Not supported.</span></span>|

<span data-ttu-id="1cf82-117">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1cf82-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1cf82-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1cf82-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="1cf82-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cf82-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="1cf82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf82-120">Request headers</span></span>
|<span data-ttu-id="1cf82-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1cf82-121">Name</span></span>|<span data-ttu-id="1cf82-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cf82-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1cf82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cf82-123">Authorization</span></span>|<span data-ttu-id="1cf82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cf82-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cf82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf82-126">Request body</span></span>
<span data-ttu-id="1cf82-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cf82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cf82-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf82-128">Response</span></span>

<span data-ttu-id="1cf82-129">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cf82-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cf82-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cf82-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cf82-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf82-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="1cf82-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf82-132">Response</span></span>
<span data-ttu-id="1cf82-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cf82-133">The following is an example of the response.</span></span>

<span data-ttu-id="1cf82-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cf82-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

