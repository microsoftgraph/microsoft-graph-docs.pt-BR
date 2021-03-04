---
title: Criar emailAuthenticationMethod
description: Crie um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b9ec2d40253faa72fd1f8d354de2649c4487e47e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436320"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="f938a-103">Criar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f938a-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="f938a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f938a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f938a-105">Definir o objeto [emailAuthenticationMethod de](../resources/emailauthenticationmethod.md) um usuário.</span><span class="sxs-lookup"><span data-stu-id="f938a-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="f938a-106">A autenticação de email é um método de redefinição de senha de autoatendados.</span><span class="sxs-lookup"><span data-stu-id="f938a-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="f938a-107">Um usuário pode ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="f938a-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="f938a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f938a-108">Permissions</span></span>
<span data-ttu-id="f938a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f938a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f938a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f938a-111">Permission type</span></span>|<span data-ttu-id="f938a-112">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="f938a-112">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="f938a-113">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="f938a-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="f938a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f938a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f938a-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f938a-115">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="f938a-116">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f938a-116">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f938a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f938a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f938a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f938a-118">Not supported.</span></span> | <span data-ttu-id="f938a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f938a-119">Not supported.</span></span> |
| <span data-ttu-id="f938a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f938a-120">Application</span></span>                            | <span data-ttu-id="f938a-121">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="f938a-121">Not applicable.</span></span> | <span data-ttu-id="f938a-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f938a-122">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f938a-123">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f938a-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="f938a-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f938a-124">Global admin</span></span>
* <span data-ttu-id="f938a-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="f938a-125">Privileged authentication admin</span></span>
* <span data-ttu-id="f938a-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="f938a-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f938a-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f938a-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="f938a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f938a-128">Request headers</span></span>
|<span data-ttu-id="f938a-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f938a-129">Name</span></span>|<span data-ttu-id="f938a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f938a-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f938a-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f938a-131">Authorization</span></span>|<span data-ttu-id="f938a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f938a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f938a-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f938a-134">Content-Type</span></span>|<span data-ttu-id="f938a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f938a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f938a-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f938a-137">Request body</span></span>
<span data-ttu-id="f938a-138">No corpo da solicitação, fornece uma representação JSON do [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.</span><span class="sxs-lookup"><span data-stu-id="f938a-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="f938a-139">A tabela a seguir mostra as propriedades que são necessárias ao criar [o emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="f938a-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="f938a-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f938a-140">Property</span></span>|<span data-ttu-id="f938a-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="f938a-141">Type</span></span>|<span data-ttu-id="f938a-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f938a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f938a-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f938a-143">emailAddress</span></span>|<span data-ttu-id="f938a-144">String</span><span class="sxs-lookup"><span data-stu-id="f938a-144">String</span></span>|<span data-ttu-id="f938a-145">Endereço de email</span><span class="sxs-lookup"><span data-stu-id="f938a-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="f938a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f938a-146">Response</span></span>

<span data-ttu-id="f938a-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f938a-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f938a-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f938a-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f938a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f938a-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f938a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f938a-150">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="f938a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f938a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f938a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f938a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f938a-153">C#</span><span class="sxs-lookup"><span data-stu-id="f938a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f938a-154">Java</span><span class="sxs-lookup"><span data-stu-id="f938a-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f938a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f938a-155">Response</span></span>
<span data-ttu-id="f938a-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f938a-156">The following is an example of the response.</span></span>

<span data-ttu-id="f938a-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f938a-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
