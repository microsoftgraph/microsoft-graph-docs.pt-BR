---
title: Criar emailAuthenticationMethod
description: Criar um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 52aabdcd45791e1ba1d2dcfc1d9faa63b7dda37a
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522479"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="963ee-103">Criar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="963ee-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="963ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="963ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="963ee-105">Definir o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="963ee-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="963ee-106">A autenticação de email é um método de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="963ee-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="963ee-107">Um usuário pode ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="963ee-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="963ee-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="963ee-108">Permissions</span></span>
<span data-ttu-id="963ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="963ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="963ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="963ee-111">Permission type</span></span>|<span data-ttu-id="963ee-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="963ee-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="963ee-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="963ee-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="963ee-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="963ee-114">Delegated (work or school account)</span></span>|<span data-ttu-id="963ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="963ee-115">Not supported.</span></span>|<span data-ttu-id="963ee-116">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="963ee-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="963ee-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="963ee-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="963ee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="963ee-118">Not supported.</span></span>|<span data-ttu-id="963ee-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="963ee-119">Not supported.</span></span>
|<span data-ttu-id="963ee-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="963ee-120">Application</span></span>|<span data-ttu-id="963ee-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="963ee-121">Not supported.</span></span>|<span data-ttu-id="963ee-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="963ee-122">Not supported.</span></span>

<span data-ttu-id="963ee-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="963ee-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="963ee-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="963ee-124">Global admin</span></span>
* <span data-ttu-id="963ee-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="963ee-125">Privileged authentication admin</span></span>
* <span data-ttu-id="963ee-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="963ee-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="963ee-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="963ee-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="963ee-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="963ee-128">Request headers</span></span>
|<span data-ttu-id="963ee-129">Nome</span><span class="sxs-lookup"><span data-stu-id="963ee-129">Name</span></span>|<span data-ttu-id="963ee-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="963ee-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="963ee-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="963ee-131">Authorization</span></span>|<span data-ttu-id="963ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="963ee-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="963ee-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="963ee-134">Content-Type</span></span>|<span data-ttu-id="963ee-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="963ee-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="963ee-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="963ee-137">Request body</span></span>
<span data-ttu-id="963ee-138">No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.</span><span class="sxs-lookup"><span data-stu-id="963ee-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="963ee-139">A tabela a seguir mostra as propriedades que são necessárias ao criar [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="963ee-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="963ee-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="963ee-140">Property</span></span>|<span data-ttu-id="963ee-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="963ee-141">Type</span></span>|<span data-ttu-id="963ee-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="963ee-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="963ee-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="963ee-143">emailAddress</span></span>|<span data-ttu-id="963ee-144">String</span><span class="sxs-lookup"><span data-stu-id="963ee-144">String</span></span>|<span data-ttu-id="963ee-145">Endereço de email</span><span class="sxs-lookup"><span data-stu-id="963ee-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="963ee-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="963ee-146">Response</span></span>

<span data-ttu-id="963ee-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="963ee-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="963ee-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="963ee-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="963ee-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="963ee-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="963ee-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="963ee-150">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="963ee-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="963ee-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="963ee-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="963ee-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="963ee-153">C#</span><span class="sxs-lookup"><span data-stu-id="963ee-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="963ee-154">Java</span><span class="sxs-lookup"><span data-stu-id="963ee-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="963ee-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="963ee-155">Response</span></span>
<span data-ttu-id="963ee-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="963ee-156">The following is an example of the response.</span></span>

<span data-ttu-id="963ee-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="963ee-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
