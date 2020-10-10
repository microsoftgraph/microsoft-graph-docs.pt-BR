---
title: Criar emailAuthenticationMethod
description: Criar um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9d00dd6d8197be3817f1129d7a8e83522eb71634
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418185"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="0208d-103">Criar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0208d-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="0208d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0208d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0208d-105">Definir o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0208d-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="0208d-106">A autenticação de email é um método de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="0208d-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="0208d-107">Um usuário pode ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="0208d-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="0208d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0208d-108">Permissions</span></span>
<span data-ttu-id="0208d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0208d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0208d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0208d-111">Permission type</span></span>|<span data-ttu-id="0208d-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="0208d-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="0208d-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0208d-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="0208d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0208d-114">Delegated (work or school account)</span></span>|<span data-ttu-id="0208d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0208d-115">Not supported.</span></span>|<span data-ttu-id="0208d-116">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0208d-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="0208d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0208d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0208d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0208d-118">Not supported.</span></span>|<span data-ttu-id="0208d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0208d-119">Not supported.</span></span>
|<span data-ttu-id="0208d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0208d-120">Application</span></span>|<span data-ttu-id="0208d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0208d-121">Not supported.</span></span>|<span data-ttu-id="0208d-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0208d-122">Not supported.</span></span>

<span data-ttu-id="0208d-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="0208d-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0208d-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0208d-124">Global admin</span></span>
* <span data-ttu-id="0208d-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="0208d-125">Global reader</span></span>
* <span data-ttu-id="0208d-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="0208d-126">Privileged authentication admin</span></span>
* <span data-ttu-id="0208d-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="0208d-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0208d-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0208d-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="0208d-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0208d-129">Request headers</span></span>
|<span data-ttu-id="0208d-130">Nome</span><span class="sxs-lookup"><span data-stu-id="0208d-130">Name</span></span>|<span data-ttu-id="0208d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0208d-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0208d-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0208d-132">Authorization</span></span>|<span data-ttu-id="0208d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0208d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0208d-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0208d-135">Content-Type</span></span>|<span data-ttu-id="0208d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0208d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0208d-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0208d-138">Request body</span></span>
<span data-ttu-id="0208d-139">No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.</span><span class="sxs-lookup"><span data-stu-id="0208d-139">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="0208d-140">A tabela a seguir mostra as propriedades que são necessárias ao criar [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="0208d-140">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="0208d-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0208d-141">Property</span></span>|<span data-ttu-id="0208d-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="0208d-142">Type</span></span>|<span data-ttu-id="0208d-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="0208d-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0208d-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0208d-144">emailAddress</span></span>|<span data-ttu-id="0208d-145">String</span><span class="sxs-lookup"><span data-stu-id="0208d-145">String</span></span>|<span data-ttu-id="0208d-146">Endereço de email</span><span class="sxs-lookup"><span data-stu-id="0208d-146">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="0208d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0208d-147">Response</span></span>

<span data-ttu-id="0208d-148">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0208d-148">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0208d-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0208d-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0208d-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0208d-150">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="0208d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0208d-151">Response</span></span>
<span data-ttu-id="0208d-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0208d-152">The following is an example of the response.</span></span>

<span data-ttu-id="0208d-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0208d-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
