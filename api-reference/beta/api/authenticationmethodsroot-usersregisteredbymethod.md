---
title: 'authenticationMethodsRoot: usersRegisteredByMethod'
description: Obter o número de usuários registrados para cada método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 684603da36a4d5dcf08fc575042b49055e581e7b
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052549"
---
# <a name="authenticationmethodsroot-usersregisteredbymethod"></a><span data-ttu-id="f67f4-103">authenticationMethodsRoot: usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="f67f4-103">authenticationMethodsRoot: usersRegisteredByMethod</span></span>
<span data-ttu-id="f67f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f67f4-105">Obter o número de usuários registrados para cada método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f67f4-105">Get the number of users registered for each authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="f67f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f67f4-106">Permissions</span></span>
<span data-ttu-id="f67f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f67f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f67f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f67f4-109">Permission type</span></span>|<span data-ttu-id="f67f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f67f4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f67f4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f67f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f67f4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f67f4-112">Reports.Read.All</span></span>|
|<span data-ttu-id="f67f4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f67f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f67f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67f4-114">Not supported.</span></span>|
|<span data-ttu-id="f67f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f67f4-115">Application</span></span>|<span data-ttu-id="f67f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67f4-116">Not supported.</span></span>|

<span data-ttu-id="f67f4-117">Para acessar a API, [uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) é necessária:</span><span class="sxs-lookup"><span data-stu-id="f67f4-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="f67f4-118">Leitor de relatórios</span><span class="sxs-lookup"><span data-stu-id="f67f4-118">Reports reader</span></span>
* <span data-ttu-id="f67f4-119">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="f67f4-119">Security reader</span></span>
* <span data-ttu-id="f67f4-120">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="f67f4-120">Security admin</span></span>
* <span data-ttu-id="f67f4-121">Leitor global</span><span class="sxs-lookup"><span data-stu-id="f67f4-121">Global reader</span></span>
* <span data-ttu-id="f67f4-122">Administração global</span><span class="sxs-lookup"><span data-stu-id="f67f4-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f67f4-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f67f4-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByMethod
```

## <a name="function-parameters"></a><span data-ttu-id="f67f4-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f67f4-124">Function parameters</span></span>
<span data-ttu-id="f67f4-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f67f4-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f67f4-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f67f4-126">Parameter</span></span>|<span data-ttu-id="f67f4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f67f4-127">Type</span></span>|<span data-ttu-id="f67f4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67f4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67f4-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="f67f4-129">includedUserTypes</span></span>|<span data-ttu-id="f67f4-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="f67f4-130">includedUserTypes</span></span>|<span data-ttu-id="f67f4-131">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="f67f4-131">User type.</span></span> <span data-ttu-id="f67f4-132">Os valores possíveis são: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="f67f4-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="f67f4-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="f67f4-133">includedUserRoles</span></span>|<span data-ttu-id="f67f4-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="f67f4-134">includedUserRoles</span></span>|<span data-ttu-id="f67f4-135">Tipo de função de usuário.</span><span class="sxs-lookup"><span data-stu-id="f67f4-135">User role type.</span></span> <span data-ttu-id="f67f4-136">Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="f67f4-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="f67f4-137">O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:</span><span class="sxs-lookup"><span data-stu-id="f67f4-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="f67f4-138">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f67f4-138">Global admin</span></span>
* <span data-ttu-id="f67f4-139">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="f67f4-139">Security admin</span></span>
* <span data-ttu-id="f67f4-140">Administrador de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="f67f4-140">Conditional Access admin</span></span>
* <span data-ttu-id="f67f4-141">Administrador do Exchange</span><span class="sxs-lookup"><span data-stu-id="f67f4-141">Exchange admin</span></span>
* <span data-ttu-id="f67f4-142">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="f67f4-142">SharePoint admin</span></span>
* <span data-ttu-id="f67f4-143">Administrador de help desk</span><span class="sxs-lookup"><span data-stu-id="f67f4-143">Helpdesk admin</span></span>
* <span data-ttu-id="f67f4-144">Administrador de faturamento</span><span class="sxs-lookup"><span data-stu-id="f67f4-144">Billing admin</span></span>
* <span data-ttu-id="f67f4-145">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="f67f4-145">User admin</span></span>
* <span data-ttu-id="f67f4-146">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="f67f4-146">Authentication admin</span></span>

<span data-ttu-id="f67f4-147">O valor inclui todas as funções de administrador do `admin` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f67f4-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f67f4-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f67f4-148">Request headers</span></span>
|<span data-ttu-id="f67f4-149">Nome</span><span class="sxs-lookup"><span data-stu-id="f67f4-149">Name</span></span>|<span data-ttu-id="f67f4-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67f4-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f67f4-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="f67f4-151">Authorization</span></span>|<span data-ttu-id="f67f4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f67f4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f67f4-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f67f4-154">Request body</span></span>
<span data-ttu-id="f67f4-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f67f4-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f67f4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67f4-156">Response</span></span>

<span data-ttu-id="f67f4-157">Se tiver êxito, esta função retornará um código de resposta e um `200 OK` [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f67f4-157">If successful, this function returns a `200 OK` response code and a [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f67f4-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f67f4-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f67f4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f67f4-159">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbymethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')
```


### <a name="response"></a><span data-ttu-id="f67f4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67f4-160">Response</span></span>
<span data-ttu-id="f67f4-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f67f4-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationMethodCounts": [{
            "authenticationMethod": "password",
            "userCount": 12209
        },
        {
            "authenticationMethod": "windowsHelloForBusiness",
            "userCount": 223
        },
        {
            "authenticationMethod": "mobilePhone",
            "userCount": 4234
        }
    ]
}
```
