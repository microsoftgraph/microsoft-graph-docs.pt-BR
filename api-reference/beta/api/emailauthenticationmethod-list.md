---
title: Listar emailAuthenticationMethods
description: Obtenha uma lista dos objetos emailAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92fdd0b55eb10264710550dae63aba6afddeff0c
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418184"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="abd49-103">Listar emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="abd49-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="abd49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abd49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abd49-105">Recupere uma lista de objetos de [método de autenticação de email](../resources/emailauthenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="abd49-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="abd49-106">Essa chamada só retornará um único objeto, pois apenas um método de email pode ser definido nos usuários.</span><span class="sxs-lookup"><span data-stu-id="abd49-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="abd49-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="abd49-107">Permissions</span></span>
<span data-ttu-id="abd49-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abd49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abd49-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abd49-110">Permission type</span></span>|<span data-ttu-id="abd49-111">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="abd49-111">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="abd49-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abd49-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="abd49-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abd49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abd49-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="abd49-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="abd49-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="abd49-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="abd49-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abd49-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd49-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abd49-117">Not supported.</span></span>|<span data-ttu-id="abd49-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abd49-118">Not supported.</span></span>
|<span data-ttu-id="abd49-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abd49-119">Application</span></span>|<span data-ttu-id="abd49-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abd49-120">Not supported.</span></span>|<span data-ttu-id="abd49-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abd49-121">Not supported.</span></span>

<span data-ttu-id="abd49-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="abd49-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="abd49-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="abd49-123">Global admin</span></span>
* <span data-ttu-id="abd49-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="abd49-124">Global reader</span></span>
* <span data-ttu-id="abd49-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="abd49-125">Privileged authentication admin</span></span>
* <span data-ttu-id="abd49-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="abd49-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="abd49-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abd49-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abd49-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abd49-128">Optional query parameters</span></span>
<span data-ttu-id="abd49-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abd49-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abd49-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abd49-130">Request headers</span></span>
|<span data-ttu-id="abd49-131">Nome</span><span class="sxs-lookup"><span data-stu-id="abd49-131">Name</span></span>|<span data-ttu-id="abd49-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="abd49-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abd49-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="abd49-133">Authorization</span></span>|<span data-ttu-id="abd49-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="abd49-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd49-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abd49-135">Request body</span></span>
<span data-ttu-id="abd49-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abd49-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abd49-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="abd49-137">Response</span></span>

<span data-ttu-id="abd49-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abd49-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abd49-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="abd49-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="abd49-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abd49-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```


### <a name="response"></a><span data-ttu-id="abd49-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="abd49-141">Response</span></span>
<span data-ttu-id="abd49-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="abd49-142">The following is an example of the response.</span></span>

<span data-ttu-id="abd49-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="abd49-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```

