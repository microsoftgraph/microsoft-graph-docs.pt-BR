---
title: 'authenticationMethodsRoot: usersRegisteredByFeature'
description: Obter o número de usuários capazes de autenticação multifa factor, redefinição de senha de autoatendado e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: a70832426dfc9b6fbadddd070d3531d52d515583
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092331"
---
# <a name="authenticationmethodsroot-usersregisteredbyfeature"></a><span data-ttu-id="55273-103">authenticationMethodsRoot: usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="55273-103">authenticationMethodsRoot: usersRegisteredByFeature</span></span>
<span data-ttu-id="55273-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55273-105">Obter o número de usuários capazes de autenticação multifa factor, redefinição de senha de autoatendado e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="55273-105">Get the number of users capable of multi-factor authentication, self-service password reset, and passwordless authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="55273-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55273-106">Permissions</span></span>
<span data-ttu-id="55273-107">As permissões a seguir são necessárias para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="55273-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="55273-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55273-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55273-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55273-109">Permission type</span></span>|<span data-ttu-id="55273-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55273-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55273-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55273-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55273-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55273-112">Reports.Read.All</span></span>|
|<span data-ttu-id="55273-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55273-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55273-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55273-114">Not supported.</span></span>|
|<span data-ttu-id="55273-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55273-115">Application</span></span>|<span data-ttu-id="55273-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55273-116">Not supported.</span></span>|

<span data-ttu-id="55273-117">Para acessar a API, [uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) é necessária:</span><span class="sxs-lookup"><span data-stu-id="55273-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="55273-118">Leitor de relatórios</span><span class="sxs-lookup"><span data-stu-id="55273-118">Reports reader</span></span>
* <span data-ttu-id="55273-119">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="55273-119">Security reader</span></span>
* <span data-ttu-id="55273-120">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="55273-120">Security admin</span></span>
* <span data-ttu-id="55273-121">Leitor global</span><span class="sxs-lookup"><span data-stu-id="55273-121">Global reader</span></span>
* <span data-ttu-id="55273-122">Administração global</span><span class="sxs-lookup"><span data-stu-id="55273-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="55273-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55273-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByFeature
```

## <a name="function-parameters"></a><span data-ttu-id="55273-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="55273-124">Function parameters</span></span>
<span data-ttu-id="55273-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="55273-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="55273-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55273-126">Parameter</span></span>|<span data-ttu-id="55273-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="55273-127">Type</span></span>|<span data-ttu-id="55273-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="55273-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55273-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="55273-129">includedUserTypes</span></span>|<span data-ttu-id="55273-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="55273-130">includedUserTypes</span></span>|<span data-ttu-id="55273-131">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="55273-131">User type.</span></span> <span data-ttu-id="55273-132">Os valores possíveis são: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="55273-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="55273-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="55273-133">includedUserRoles</span></span>|<span data-ttu-id="55273-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="55273-134">includedUserRoles</span></span>|<span data-ttu-id="55273-135">Tipo de função de usuário.</span><span class="sxs-lookup"><span data-stu-id="55273-135">User role type.</span></span> <span data-ttu-id="55273-136">Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="55273-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="55273-137">O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:</span><span class="sxs-lookup"><span data-stu-id="55273-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="55273-138">Administrador global</span><span class="sxs-lookup"><span data-stu-id="55273-138">Global admin</span></span>
* <span data-ttu-id="55273-139">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="55273-139">Security admin</span></span>
* <span data-ttu-id="55273-140">Administrador de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="55273-140">Conditional Access admin</span></span>
* <span data-ttu-id="55273-141">Administrador do Exchange</span><span class="sxs-lookup"><span data-stu-id="55273-141">Exchange admin</span></span>
* <span data-ttu-id="55273-142">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="55273-142">SharePoint admin</span></span>
* <span data-ttu-id="55273-143">Administrador de help desk</span><span class="sxs-lookup"><span data-stu-id="55273-143">Helpdesk admin</span></span>
* <span data-ttu-id="55273-144">Administrador de faturamento</span><span class="sxs-lookup"><span data-stu-id="55273-144">Billing admin</span></span>
* <span data-ttu-id="55273-145">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="55273-145">User admin</span></span>
* <span data-ttu-id="55273-146">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="55273-146">Authentication admin</span></span>

<span data-ttu-id="55273-147">O valor inclui todas as funções de administrador do `admin` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="55273-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="55273-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55273-148">Request headers</span></span>
|<span data-ttu-id="55273-149">Nome</span><span class="sxs-lookup"><span data-stu-id="55273-149">Name</span></span>|<span data-ttu-id="55273-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="55273-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55273-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="55273-151">Authorization</span></span>|<span data-ttu-id="55273-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55273-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55273-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55273-154">Request body</span></span>
<span data-ttu-id="55273-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55273-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55273-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="55273-156">Response</span></span>

<span data-ttu-id="55273-157">Se tiver êxito, esta função retornará um código de resposta e um `200 OK` [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55273-157">If successful, this function returns a `200 OK` response code and a [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55273-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55273-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55273-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55273-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="55273-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="55273-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbyfeature"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')
```
# <a name="c"></a>[<span data-ttu-id="55273-161">C#</span><span class="sxs-lookup"><span data-stu-id="55273-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/authenticationmethodsroot-usersregisteredbyfeature-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55273-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55273-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/authenticationmethodsroot-usersregisteredbyfeature-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55273-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55273-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/authenticationmethodsroot-usersregisteredbyfeature-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55273-164">Java</span><span class="sxs-lookup"><span data-stu-id="55273-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/authenticationmethodsroot-usersregisteredbyfeature-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="55273-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="55273-165">Response</span></span>
<span data-ttu-id="55273-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55273-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
    "totalUserCount": 23123,
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationFeatureCounts": [{
            "feature": "ssprRegistered",
            "userCount": 23423
        },
        {
            "feature": "ssprEnabled",
            "userCount": 4234
        },
        {
            "feature": "ssprCapable",
            "userCount": 4234
        }, {
            "feature": "passwordlessRegistered",
            "userCount": 323
        },
        {
            "feature": "mfaCapable",
            "userCount": 3345
        }
    ]
}
```
