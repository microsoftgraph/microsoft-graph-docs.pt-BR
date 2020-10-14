---
title: Atualizar emailAuthenticationMethod
description: Atualiza as propriedades de um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc4fc3c7900482e4444465a406e7c8b4319bcf0f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458114"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="d8d48-103">Atualizar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d8d48-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="d8d48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d48-105">Atualize o endereço de email de um usuário associado a um objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="d8d48-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8d48-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8d48-106">Permissions</span></span>
<span data-ttu-id="d8d48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8d48-109">Permission type</span></span>|<span data-ttu-id="d8d48-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8d48-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="d8d48-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8d48-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="d8d48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8d48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8d48-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d48-113">Not supported.</span></span>|<span data-ttu-id="d8d48-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d8d48-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="d8d48-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8d48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8d48-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d48-116">Not supported.</span></span>|<span data-ttu-id="d8d48-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d48-117">Not supported.</span></span>
|<span data-ttu-id="d8d48-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8d48-118">Application</span></span>|<span data-ttu-id="d8d48-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d48-119">Not supported.</span></span>|<span data-ttu-id="d8d48-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d48-120">Not supported.</span></span>

<span data-ttu-id="d8d48-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="d8d48-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d8d48-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d8d48-122">Global admin</span></span>
* <span data-ttu-id="d8d48-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="d8d48-123">Global reader</span></span>
* <span data-ttu-id="d8d48-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d8d48-124">Privileged authentication admin</span></span>
* <span data-ttu-id="d8d48-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="d8d48-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d8d48-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d48-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8d48-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d48-127">Request headers</span></span>
|<span data-ttu-id="d8d48-128">Nome</span><span class="sxs-lookup"><span data-stu-id="d8d48-128">Name</span></span>|<span data-ttu-id="d8d48-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d48-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d8d48-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8d48-130">Authorization</span></span>|<span data-ttu-id="d8d48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8d48-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8d48-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8d48-133">Content-Type</span></span>|<span data-ttu-id="d8d48-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8d48-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d48-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d48-136">Request body</span></span>
<span data-ttu-id="d8d48-137">No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email atualizado.</span><span class="sxs-lookup"><span data-stu-id="d8d48-137">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="d8d48-138">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="d8d48-138">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="d8d48-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d48-139">Property</span></span>|<span data-ttu-id="d8d48-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d48-140">Type</span></span>|<span data-ttu-id="d8d48-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d48-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8d48-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d8d48-142">emailAddress</span></span>|<span data-ttu-id="d8d48-143">String</span><span class="sxs-lookup"><span data-stu-id="d8d48-143">String</span></span>|<span data-ttu-id="d8d48-144">Endereço de email atualizado</span><span class="sxs-lookup"><span data-stu-id="d8d48-144">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="d8d48-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d48-145">Response</span></span>

<span data-ttu-id="d8d48-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d48-146">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8d48-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8d48-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8d48-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d48-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d8d48-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d48-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="d8d48-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8d48-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8d48-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8d48-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d8d48-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d48-152">Response</span></span>

<span data-ttu-id="d8d48-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d48-153">The following is an example of the response.</span></span>

<span data-ttu-id="d8d48-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8d48-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
