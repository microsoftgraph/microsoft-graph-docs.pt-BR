---
title: Criar emailAuthenticationMethod
description: Criar um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fa084db81af3677f5a6e12c6d90020178653b4f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458124"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="fccdd-103">Criar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fccdd-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="fccdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fccdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fccdd-105">Definir o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fccdd-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="fccdd-106">A autenticação de email é um método de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="fccdd-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="fccdd-107">Um usuário pode ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="fccdd-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="fccdd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fccdd-108">Permissions</span></span>
<span data-ttu-id="fccdd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fccdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fccdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fccdd-111">Permission type</span></span>|<span data-ttu-id="fccdd-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="fccdd-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="fccdd-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fccdd-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="fccdd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fccdd-114">Delegated (work or school account)</span></span>|<span data-ttu-id="fccdd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fccdd-115">Not supported.</span></span>|<span data-ttu-id="fccdd-116">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fccdd-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="fccdd-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fccdd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fccdd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fccdd-118">Not supported.</span></span>|<span data-ttu-id="fccdd-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fccdd-119">Not supported.</span></span>
|<span data-ttu-id="fccdd-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fccdd-120">Application</span></span>|<span data-ttu-id="fccdd-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fccdd-121">Not supported.</span></span>|<span data-ttu-id="fccdd-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fccdd-122">Not supported.</span></span>

<span data-ttu-id="fccdd-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="fccdd-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="fccdd-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fccdd-124">Global admin</span></span>
* <span data-ttu-id="fccdd-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="fccdd-125">Global reader</span></span>
* <span data-ttu-id="fccdd-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="fccdd-126">Privileged authentication admin</span></span>
* <span data-ttu-id="fccdd-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="fccdd-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="fccdd-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fccdd-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="fccdd-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fccdd-129">Request headers</span></span>
|<span data-ttu-id="fccdd-130">Nome</span><span class="sxs-lookup"><span data-stu-id="fccdd-130">Name</span></span>|<span data-ttu-id="fccdd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fccdd-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fccdd-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="fccdd-132">Authorization</span></span>|<span data-ttu-id="fccdd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fccdd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fccdd-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fccdd-135">Content-Type</span></span>|<span data-ttu-id="fccdd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fccdd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fccdd-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fccdd-138">Request body</span></span>
<span data-ttu-id="fccdd-139">No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.</span><span class="sxs-lookup"><span data-stu-id="fccdd-139">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="fccdd-140">A tabela a seguir mostra as propriedades que são necessárias ao criar [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="fccdd-140">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="fccdd-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fccdd-141">Property</span></span>|<span data-ttu-id="fccdd-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="fccdd-142">Type</span></span>|<span data-ttu-id="fccdd-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="fccdd-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fccdd-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fccdd-144">emailAddress</span></span>|<span data-ttu-id="fccdd-145">String</span><span class="sxs-lookup"><span data-stu-id="fccdd-145">String</span></span>|<span data-ttu-id="fccdd-146">Endereço de email</span><span class="sxs-lookup"><span data-stu-id="fccdd-146">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="fccdd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fccdd-147">Response</span></span>

<span data-ttu-id="fccdd-148">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fccdd-148">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fccdd-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fccdd-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fccdd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fccdd-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fccdd-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="fccdd-151">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fccdd-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fccdd-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fccdd-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fccdd-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fccdd-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fccdd-154">Response</span></span>
<span data-ttu-id="fccdd-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fccdd-155">The following is an example of the response.</span></span>

<span data-ttu-id="fccdd-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fccdd-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
