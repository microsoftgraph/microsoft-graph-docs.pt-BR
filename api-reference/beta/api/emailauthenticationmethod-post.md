---
title: Criar emailAuthenticationMethod
description: Criar um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 832869fcc3e60f3b9497984b79851d6388a84fc1
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796328"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="62952-103">Criar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="62952-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="62952-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62952-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62952-105">Definir o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="62952-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="62952-106">A autenticação de email é um método de redefinição de senha de autoatendado.</span><span class="sxs-lookup"><span data-stu-id="62952-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="62952-107">Um usuário pode ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="62952-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="62952-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="62952-108">Permissions</span></span>
<span data-ttu-id="62952-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62952-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62952-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62952-111">Permission type</span></span>|<span data-ttu-id="62952-112">Permissões atuando por si mesmo (do mais para o menos privilegiado)</span><span class="sxs-lookup"><span data-stu-id="62952-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="62952-113">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="62952-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="62952-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62952-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="62952-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62952-115">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="62952-116">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62952-116">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="62952-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62952-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62952-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62952-118">Not supported.</span></span> | <span data-ttu-id="62952-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62952-119">Not supported.</span></span> |
| <span data-ttu-id="62952-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62952-120">Application</span></span>                            | <span data-ttu-id="62952-121">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="62952-121">Not applicable.</span></span> | <span data-ttu-id="62952-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62952-122">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="62952-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="62952-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="62952-124">Administração global</span><span class="sxs-lookup"><span data-stu-id="62952-124">Global admin</span></span>
* <span data-ttu-id="62952-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="62952-125">Privileged authentication admin</span></span>
* <span data-ttu-id="62952-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="62952-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="62952-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="62952-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62952-128">Request headers</span></span>
|<span data-ttu-id="62952-129">Nome</span><span class="sxs-lookup"><span data-stu-id="62952-129">Name</span></span>|<span data-ttu-id="62952-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="62952-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62952-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="62952-131">Authorization</span></span>|<span data-ttu-id="62952-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62952-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62952-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62952-134">Content-Type</span></span>|<span data-ttu-id="62952-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62952-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62952-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62952-137">Request body</span></span>
<span data-ttu-id="62952-138">No corpo da solicitação, fornece uma representação JSON do [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.</span><span class="sxs-lookup"><span data-stu-id="62952-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="62952-139">A tabela a seguir mostra as propriedades que são necessárias ao criar [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="62952-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="62952-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62952-140">Property</span></span>|<span data-ttu-id="62952-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="62952-141">Type</span></span>|<span data-ttu-id="62952-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="62952-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62952-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="62952-143">emailAddress</span></span>|<span data-ttu-id="62952-144">String</span><span class="sxs-lookup"><span data-stu-id="62952-144">String</span></span>|<span data-ttu-id="62952-145">Email</span><span class="sxs-lookup"><span data-stu-id="62952-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="62952-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="62952-146">Response</span></span>

<span data-ttu-id="62952-147">Se bem-sucedido, este método retorna um código de resposta e um novo `201 Created` [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62952-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62952-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62952-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62952-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62952-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="62952-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="62952-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="62952-153">C#</span><span class="sxs-lookup"><span data-stu-id="62952-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62952-154">Java</span><span class="sxs-lookup"><span data-stu-id="62952-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="62952-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="62952-155">Response</span></span>
<span data-ttu-id="62952-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62952-156">The following is an example of the response.</span></span>

<span data-ttu-id="62952-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62952-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
