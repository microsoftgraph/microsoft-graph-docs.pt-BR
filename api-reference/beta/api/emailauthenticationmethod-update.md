---
title: Atualizar emailAuthenticationMethod
description: Atualizar as propriedades de um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e1509426af1d967c1fa6e6ed9ec7999a50afb04
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796426"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="7bd8b-103">Atualizar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7bd8b-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="7bd8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bd8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bd8b-105">Atualize o endereço de email de um usuário associado a um objeto de método [de autenticação de email.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bd8b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7bd8b-106">Permissions</span></span>
<span data-ttu-id="7bd8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bd8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bd8b-109">Permission type</span></span>|<span data-ttu-id="7bd8b-110">Permissões atuando por si mesmo (do mais para o menos privilegiado)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="7bd8b-111">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="7bd8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bd8b-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bd8b-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="7bd8b-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd8b-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="7bd8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bd8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-116">Not supported.</span></span> | <span data-ttu-id="7bd8b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-117">Not supported.</span></span> |
| <span data-ttu-id="7bd8b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bd8b-118">Application</span></span>                            | <span data-ttu-id="7bd8b-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-119">Not applicable.</span></span> | <span data-ttu-id="7bd8b-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd8b-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="7bd8b-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="7bd8b-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="7bd8b-122">Administração global</span><span class="sxs-lookup"><span data-stu-id="7bd8b-122">Global admin</span></span>
* <span data-ttu-id="7bd8b-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="7bd8b-123">Privileged authentication admin</span></span>
* <span data-ttu-id="7bd8b-124">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="7bd8b-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7bd8b-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bd8b-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7bd8b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bd8b-126">Request headers</span></span>
|<span data-ttu-id="7bd8b-127">Nome</span><span class="sxs-lookup"><span data-stu-id="7bd8b-127">Name</span></span>|<span data-ttu-id="7bd8b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bd8b-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bd8b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bd8b-129">Authorization</span></span>|<span data-ttu-id="7bd8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7bd8b-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bd8b-132">Content-Type</span></span>|<span data-ttu-id="7bd8b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd8b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bd8b-135">Request body</span></span>
<span data-ttu-id="7bd8b-136">No corpo da solicitação, fornece uma representação JSON do [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email atualizado.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="7bd8b-137">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="7bd8b-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="7bd8b-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bd8b-138">Property</span></span>|<span data-ttu-id="7bd8b-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bd8b-139">Type</span></span>|<span data-ttu-id="7bd8b-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bd8b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd8b-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7bd8b-141">emailAddress</span></span>|<span data-ttu-id="7bd8b-142">String</span><span class="sxs-lookup"><span data-stu-id="7bd8b-142">String</span></span>|<span data-ttu-id="7bd8b-143">Endereço de email atualizado</span><span class="sxs-lookup"><span data-stu-id="7bd8b-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="7bd8b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bd8b-144">Response</span></span>

<span data-ttu-id="7bd8b-145">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bd8b-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7bd8b-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bd8b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bd8b-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7bd8b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bd8b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PUT https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7bd8b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bd8b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bd8b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bd8b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7bd8b-151">C#</span><span class="sxs-lookup"><span data-stu-id="7bd8b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bd8b-152">Java</span><span class="sxs-lookup"><span data-stu-id="7bd8b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7bd8b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bd8b-153">Response</span></span>

<span data-ttu-id="7bd8b-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-154">The following is an example of the response.</span></span>

<span data-ttu-id="7bd8b-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7bd8b-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
