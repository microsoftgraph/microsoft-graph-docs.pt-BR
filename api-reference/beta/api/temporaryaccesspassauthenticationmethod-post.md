---
title: Criar temporaryAccessPassAuthenticationMethod
description: Crie um novo objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d048d843c0a93dc779a0966d6a27d337251fc974
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272598"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="fb944-103">Criar temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fb944-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="fb944-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb944-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb944-105">Crie um novo [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) em um usuário.</span><span class="sxs-lookup"><span data-stu-id="fb944-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="fb944-106">Um usuário só pode ter uma Passagem de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="fb944-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="fb944-107">A senha pode ser usada entre a hora de início e término do Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="fb944-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="fb944-108">Se o usuário exigir uma nova Passagem de Acesso Temporário:</span><span class="sxs-lookup"><span data-stu-id="fb944-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="fb944-109">Embora o Acesso Temporário atual seja válido– o administrador precisa excluir o Acesso Temporário existente e criar uma nova passagem para o usuário.</span><span class="sxs-lookup"><span data-stu-id="fb944-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="fb944-110">A exclusão de uma Passagem de Acesso Temporário válida revoga as sessões do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb944-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="fb944-111">Depois que o Acesso Temporário expirar, um novo acesso temporário substituirá o acesso temporário atual e não revoga as sessões do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb944-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="fb944-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="fb944-112">Permissions</span></span>

<span data-ttu-id="fb944-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb944-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="fb944-115">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="fb944-115">Permissions acting on self</span></span>

|<span data-ttu-id="fb944-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb944-116">Permission type</span></span>      | <span data-ttu-id="fb944-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb944-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="fb944-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb944-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb944-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb944-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="fb944-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb944-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb944-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb944-121">Not supported.</span></span> |
| <span data-ttu-id="fb944-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb944-122">Application</span></span>                            | <span data-ttu-id="fb944-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb944-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="fb944-124">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="fb944-124">Permissions acting on other users</span></span>

|<span data-ttu-id="fb944-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb944-125">Permission type</span></span>      | <span data-ttu-id="fb944-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb944-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="fb944-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb944-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb944-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb944-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="fb944-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb944-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb944-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb944-130">Not supported.</span></span> |
| <span data-ttu-id="fb944-131">Application</span><span class="sxs-lookup"><span data-stu-id="fb944-131">Application</span></span>                            | <span data-ttu-id="fb944-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb944-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="fb944-133">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="fb944-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="fb944-134">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fb944-134">Global admin</span></span>
* <span data-ttu-id="fb944-135">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="fb944-135">Privileged authentication admin</span></span>
* <span data-ttu-id="fb944-136">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="fb944-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="fb944-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb944-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="fb944-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb944-138">Request headers</span></span>
|<span data-ttu-id="fb944-139">Nome</span><span class="sxs-lookup"><span data-stu-id="fb944-139">Name</span></span>|<span data-ttu-id="fb944-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb944-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb944-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb944-141">Authorization</span></span>|<span data-ttu-id="fb944-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb944-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fb944-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb944-144">Content-Type</span></span>|<span data-ttu-id="fb944-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb944-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb944-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb944-147">Request body</span></span>
<span data-ttu-id="fb944-148">No corpo da solicitação, fornece uma representação JSON do objeto [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="fb944-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="fb944-149">A tabela a seguir descreve as propriedades opcionais que podem ser usadas ao criar [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="fb944-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="fb944-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb944-150">Property</span></span>|<span data-ttu-id="fb944-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb944-151">Type</span></span>|<span data-ttu-id="fb944-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb944-152">Description</span></span>|<span data-ttu-id="fb944-153">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="fb944-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="fb944-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fb944-154">startDateTime</span></span>|<span data-ttu-id="fb944-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb944-155">DateTimeOffset</span></span>|<span data-ttu-id="fb944-156">A data e a hora em que o temporaryAccessPass se torna disponível para uso, se não for definido, o Acesso Temporário estará disponível para uso na hora de criação.</span><span class="sxs-lookup"><span data-stu-id="fb944-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="fb944-157">Não</span><span class="sxs-lookup"><span data-stu-id="fb944-157">No</span></span>|
|<span data-ttu-id="fb944-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="fb944-158">lifetimeInMinutes</span></span>|<span data-ttu-id="fb944-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fb944-159">Int32</span></span>|<span data-ttu-id="fb944-160">O tempo de vida do temporaryAccessPass em minutos, começando no momento da criação ou em startDateTime, se definido.</span><span class="sxs-lookup"><span data-stu-id="fb944-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="fb944-161">Mínimo de 10, Máximo 43200 (equivalente a 30 dias).</span><span class="sxs-lookup"><span data-stu-id="fb944-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="fb944-162">Não</span><span class="sxs-lookup"><span data-stu-id="fb944-162">No</span></span>|
|<span data-ttu-id="fb944-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="fb944-163">isUsableOnce</span></span>|<span data-ttu-id="fb944-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb944-164">Boolean</span></span>|<span data-ttu-id="fb944-165">Determina se a passagem está limitada a um uso único.</span><span class="sxs-lookup"><span data-stu-id="fb944-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="fb944-166">Se true – a passagem pode ser usada uma vez, se False – a passagem pode ser usada várias vezes dentro do tempo de vida temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="fb944-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="fb944-167">Uma Passagem de Acesso Temporário com vários usos (isUsableOnce = false), só poderá ser criada e usada para entrar se for permitida pela política de método autenticação de passagem de acesso temporário.</span><span class="sxs-lookup"><span data-stu-id="fb944-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="fb944-168">Não</span><span class="sxs-lookup"><span data-stu-id="fb944-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="fb944-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb944-169">Response</span></span>

<span data-ttu-id="fb944-170">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb944-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb944-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb944-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb944-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb944-172">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="fb944-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb944-173">Response</span></span>
<span data-ttu-id="fb944-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb944-174">**Note:** The response object shown here might be shortened for readability.</span></span>
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