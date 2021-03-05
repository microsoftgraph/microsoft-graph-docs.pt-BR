---
title: Criar temporaryAccessPassAuthenticationMethod
description: Crie um novo objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 544911076be077740d77ec45faf76a315e96e805
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475062"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="391fb-103">Criar temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="391fb-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="391fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="391fb-105">Crie um novo [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) em um usuário.</span><span class="sxs-lookup"><span data-stu-id="391fb-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="391fb-106">Um usuário só pode ter um Passe de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="391fb-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="391fb-107">A senha pode ser usada entre a hora de início e término do Passe de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="391fb-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="391fb-108">Se o usuário exigir um novo Passe de Acesso Temporário:</span><span class="sxs-lookup"><span data-stu-id="391fb-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="391fb-109">Embora o Passe de Acesso Temporário atual seja válido – o administrador precisa excluir o Passe de Acesso Temporário existente e criar uma nova passagem no usuário.</span><span class="sxs-lookup"><span data-stu-id="391fb-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="391fb-110">Excluir um Passe de Acesso Temporário válido revoga as sessões do usuário.</span><span class="sxs-lookup"><span data-stu-id="391fb-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="391fb-111">Depois que o Passe de Acesso Temporário tiver expirado – uma nova passagem de acesso temporário substitui o passe de acesso temporário atual e não revoga as sessões do usuário.</span><span class="sxs-lookup"><span data-stu-id="391fb-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="391fb-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="391fb-112">Permissions</span></span>

<span data-ttu-id="391fb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="391fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="391fb-115">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="391fb-115">Permissions acting on self</span></span>

|<span data-ttu-id="391fb-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="391fb-116">Permission type</span></span>      | <span data-ttu-id="391fb-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="391fb-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="391fb-118">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="391fb-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="391fb-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="391fb-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="391fb-120">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="391fb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391fb-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391fb-121">Not supported.</span></span> |
| <span data-ttu-id="391fb-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="391fb-122">Application</span></span>                            | <span data-ttu-id="391fb-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391fb-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="391fb-124">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="391fb-124">Permissions acting on other users</span></span>

|<span data-ttu-id="391fb-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="391fb-125">Permission type</span></span>      | <span data-ttu-id="391fb-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="391fb-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="391fb-127">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="391fb-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="391fb-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391fb-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="391fb-129">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="391fb-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391fb-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391fb-130">Not supported.</span></span> |
| <span data-ttu-id="391fb-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="391fb-131">Application</span></span>                            | <span data-ttu-id="391fb-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391fb-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="391fb-133">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="391fb-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="391fb-134">Administrador global</span><span class="sxs-lookup"><span data-stu-id="391fb-134">Global admin</span></span>
* <span data-ttu-id="391fb-135">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="391fb-135">Privileged authentication admin</span></span>
* <span data-ttu-id="391fb-136">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="391fb-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="391fb-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="391fb-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="391fb-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="391fb-138">Request headers</span></span>
|<span data-ttu-id="391fb-139">Nome</span><span class="sxs-lookup"><span data-stu-id="391fb-139">Name</span></span>|<span data-ttu-id="391fb-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="391fb-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="391fb-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="391fb-141">Authorization</span></span>|<span data-ttu-id="391fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391fb-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="391fb-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="391fb-144">Content-Type</span></span>|<span data-ttu-id="391fb-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391fb-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="391fb-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="391fb-147">Request body</span></span>
<span data-ttu-id="391fb-148">No corpo da solicitação, fornece uma representação JSON do [objeto temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="391fb-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="391fb-149">A tabela a seguir descreve propriedades opcionais que podem ser usadas ao criar [o temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="391fb-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="391fb-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="391fb-150">Property</span></span>|<span data-ttu-id="391fb-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="391fb-151">Type</span></span>|<span data-ttu-id="391fb-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="391fb-152">Description</span></span>|<span data-ttu-id="391fb-153">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="391fb-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="391fb-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="391fb-154">startDateTime</span></span>|<span data-ttu-id="391fb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="391fb-155">DateTimeOffset</span></span>|<span data-ttu-id="391fb-156">A data e a hora em que o temporaryAccessPass fica disponível para uso, se não definir o Passe de Acesso Temporário estará disponível para uso no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="391fb-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="391fb-157">Não</span><span class="sxs-lookup"><span data-stu-id="391fb-157">No</span></span>|
|<span data-ttu-id="391fb-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="391fb-158">lifetimeInMinutes</span></span>|<span data-ttu-id="391fb-159">Int32</span><span class="sxs-lookup"><span data-stu-id="391fb-159">Int32</span></span>|<span data-ttu-id="391fb-160">O tempo de vida do temporaryAccessPass em minutos começando na hora da criação ou em startDateTime, se definido.</span><span class="sxs-lookup"><span data-stu-id="391fb-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="391fb-161">Mínimo 10, Máximo 43200 (equivalente a 30 dias).</span><span class="sxs-lookup"><span data-stu-id="391fb-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="391fb-162">Não</span><span class="sxs-lookup"><span data-stu-id="391fb-162">No</span></span>|
|<span data-ttu-id="391fb-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="391fb-163">isUsableOnce</span></span>|<span data-ttu-id="391fb-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="391fb-164">Boolean</span></span>|<span data-ttu-id="391fb-165">Determina se a passagem está limitada a um uso único.</span><span class="sxs-lookup"><span data-stu-id="391fb-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="391fb-166">Se True – o passe pode ser usado uma vez, se False – o passe pode ser usado várias vezes dentro do tempo de vida temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="391fb-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="391fb-167">Um Passe de Acesso Temporário com vários usos (isUsableOnce = false), só poderá ser criado e usado para entrar se for permitido pela política de método Autenticação de Passagem de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="391fb-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="391fb-168">Não</span><span class="sxs-lookup"><span data-stu-id="391fb-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="391fb-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="391fb-169">Response</span></span>

<span data-ttu-id="391fb-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="391fb-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="391fb-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="391fb-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="391fb-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="391fb-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="391fb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="391fb-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
  "lifetimeInMinutes": 60,
  "isUsableOnce": false
}
```
# <a name="c"></a>[<span data-ttu-id="391fb-174">C#</span><span class="sxs-lookup"><span data-stu-id="391fb-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="391fb-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="391fb-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="391fb-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="391fb-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="391fb-177">Java</span><span class="sxs-lookup"><span data-stu-id="391fb-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="391fb-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="391fb-178">Response</span></span>
<span data-ttu-id="391fb-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="391fb-179">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```
