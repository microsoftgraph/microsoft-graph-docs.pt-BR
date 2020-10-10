---
title: Atualizar emailAuthenticationMethod
description: Atualiza as propriedades de um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9da21f027d69f12f0548f7cce720ce1bea83f577
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418183"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="1d37b-103">Atualizar emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1d37b-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="1d37b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d37b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d37b-105">Atualize o endereço de email de um usuário associado a um objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="1d37b-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d37b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d37b-106">Permissions</span></span>
<span data-ttu-id="1d37b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d37b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d37b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d37b-109">Permission type</span></span>|<span data-ttu-id="1d37b-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d37b-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="1d37b-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d37b-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="1d37b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d37b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d37b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d37b-113">Not supported.</span></span>|<span data-ttu-id="1d37b-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d37b-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="1d37b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d37b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d37b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d37b-116">Not supported.</span></span>|<span data-ttu-id="1d37b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d37b-117">Not supported.</span></span>
|<span data-ttu-id="1d37b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d37b-118">Application</span></span>|<span data-ttu-id="1d37b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d37b-119">Not supported.</span></span>|<span data-ttu-id="1d37b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d37b-120">Not supported.</span></span>

<span data-ttu-id="1d37b-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1d37b-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1d37b-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1d37b-122">Global admin</span></span>
* <span data-ttu-id="1d37b-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1d37b-123">Global reader</span></span>
* <span data-ttu-id="1d37b-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1d37b-124">Privileged authentication admin</span></span>
* <span data-ttu-id="1d37b-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="1d37b-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1d37b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d37b-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1d37b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d37b-127">Request headers</span></span>
|<span data-ttu-id="1d37b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="1d37b-128">Name</span></span>|<span data-ttu-id="1d37b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d37b-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d37b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d37b-130">Authorization</span></span>|<span data-ttu-id="1d37b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d37b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d37b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d37b-133">Content-Type</span></span>|<span data-ttu-id="1d37b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d37b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d37b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d37b-136">Request body</span></span>
<span data-ttu-id="1d37b-137">No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email atualizado.</span><span class="sxs-lookup"><span data-stu-id="1d37b-137">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="1d37b-138">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="1d37b-138">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="1d37b-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d37b-139">Property</span></span>|<span data-ttu-id="1d37b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d37b-140">Type</span></span>|<span data-ttu-id="1d37b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d37b-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d37b-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1d37b-142">emailAddress</span></span>|<span data-ttu-id="1d37b-143">String</span><span class="sxs-lookup"><span data-stu-id="1d37b-143">String</span></span>|<span data-ttu-id="1d37b-144">Endereço de email atualizado</span><span class="sxs-lookup"><span data-stu-id="1d37b-144">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="1d37b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d37b-145">Response</span></span>

<span data-ttu-id="1d37b-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d37b-146">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d37b-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d37b-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d37b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d37b-148">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="1d37b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d37b-149">Response</span></span>

<span data-ttu-id="1d37b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d37b-150">The following is an example of the response.</span></span>

<span data-ttu-id="1d37b-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d37b-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
