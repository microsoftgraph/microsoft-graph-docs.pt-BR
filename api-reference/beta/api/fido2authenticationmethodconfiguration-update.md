---
title: Atualizar fido2AuthenticationMethodConfiguration
description: Atualiza as propriedades de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4337d6d7207cdfd60c1dc16e39d7e0c5c2739cc8
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418172"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="0df06-103">Atualizar fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0df06-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="0df06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df06-105">Atualizar as propriedades de um objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , que representa a política de método de autenticação de chaves de segurança FIDO2 para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0df06-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df06-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0df06-106">Permissions</span></span>
<span data-ttu-id="0df06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0df06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0df06-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0df06-109">Permission type</span></span>|<span data-ttu-id="0df06-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0df06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0df06-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0df06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0df06-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0df06-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="0df06-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0df06-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0df06-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0df06-114">Not supported.</span></span>|
|<span data-ttu-id="0df06-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0df06-115">Application</span></span>|<span data-ttu-id="0df06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0df06-116">Not supported.</span></span>|

<span data-ttu-id="0df06-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="0df06-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0df06-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0df06-118">Global admin</span></span>
* <span data-ttu-id="0df06-119">Leitor global</span><span class="sxs-lookup"><span data-stu-id="0df06-119">Global reader</span></span>
* <span data-ttu-id="0df06-120">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="0df06-120">Privileged authentication admin</span></span>
* <span data-ttu-id="0df06-121">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="0df06-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0df06-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0df06-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="0df06-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0df06-123">Request headers</span></span>
|<span data-ttu-id="0df06-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0df06-124">Name</span></span>|<span data-ttu-id="0df06-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df06-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0df06-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0df06-126">Authorization</span></span>|<span data-ttu-id="0df06-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0df06-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0df06-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0df06-129">Content-Type</span></span>|<span data-ttu-id="0df06-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0df06-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0df06-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0df06-132">Request body</span></span>
<span data-ttu-id="0df06-133">No corpo da solicitação, forneça uma representação JSON de um objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0df06-133">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="0df06-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0df06-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0df06-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0df06-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="0df06-136">Para obter a lista de propriedades que podem ser atualizadas, consulte [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0df06-136">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="0df06-137">**Observação:** A `@odata.type` propriedade com um valor de `#microsoft.graph.fido2AuthenticationMethodConfiguration` deve ser incluída no corpo.</span><span class="sxs-lookup"><span data-stu-id="0df06-137">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="0df06-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df06-138">Response</span></span>

<span data-ttu-id="0df06-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0df06-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0df06-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0df06-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0df06-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0df06-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_fido2authenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "state": "enabled",
    "isAttestationEnforced": "true"
}
```


### <a name="response"></a><span data-ttu-id="0df06-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df06-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

