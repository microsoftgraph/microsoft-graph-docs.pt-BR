---
title: Listar fido2AuthenticationMethod
description: Recupere uma lista dos objetos fido2AuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98b078f4b79af76e2618c94f533b5d4e4b6d672f
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418168"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="aba8c-103">Listar fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aba8c-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="aba8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aba8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba8c-105">Recupere uma lista de objetos de [método de autenticação de chave de segurança FIDO2](../resources/fido2authenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="aba8c-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="aba8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aba8c-106">Permissions</span></span>
<span data-ttu-id="aba8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba8c-109">Permission type</span></span>|<span data-ttu-id="aba8c-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="aba8c-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="aba8c-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aba8c-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="aba8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aba8c-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aba8c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="aba8c-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aba8c-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="aba8c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aba8c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba8c-116">Not supported.</span></span>|<span data-ttu-id="aba8c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba8c-117">Not supported.</span></span>
|<span data-ttu-id="aba8c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba8c-118">Application</span></span>|<span data-ttu-id="aba8c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba8c-119">Not supported.</span></span>|<span data-ttu-id="aba8c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba8c-120">Not supported.</span></span>

<span data-ttu-id="aba8c-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="aba8c-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="aba8c-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="aba8c-122">Global admin</span></span>
* <span data-ttu-id="aba8c-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="aba8c-123">Global reader</span></span>
* <span data-ttu-id="aba8c-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="aba8c-124">Privileged authentication admin</span></span>
* <span data-ttu-id="aba8c-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="aba8c-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="aba8c-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aba8c-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aba8c-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aba8c-127">Optional query parameters</span></span>
<span data-ttu-id="aba8c-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aba8c-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aba8c-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aba8c-129">Request headers</span></span>
|<span data-ttu-id="aba8c-130">Nome</span><span class="sxs-lookup"><span data-stu-id="aba8c-130">Name</span></span>|<span data-ttu-id="aba8c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aba8c-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aba8c-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="aba8c-132">Authorization</span></span>|<span data-ttu-id="aba8c-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="aba8c-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aba8c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aba8c-134">Request body</span></span>
<span data-ttu-id="aba8c-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aba8c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aba8c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba8c-136">Response</span></span>

<span data-ttu-id="aba8c-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aba8c-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aba8c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aba8c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aba8c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aba8c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```


### <a name="response"></a><span data-ttu-id="aba8c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba8c-140">Response</span></span>
<span data-ttu-id="aba8c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aba8c-141">The following is an example of the response.</span></span>

<span data-ttu-id="aba8c-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aba8c-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.fido2AuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
      "id": "_jpuR-TGZgk6aQCLF3BQjA2",
      "displayName": "Blue key",
      "creationDateTime": "2020-08-10T06:25:38Z",
      "aaGuid": "c5ef55ff-ad9a-4b9f-b580-ababafe026d0",
      "model": "USB key",
      "attestationCertificates": [
          "b479e7652167f574296e76bfa76731b8ccd22ed7"
      ],
      "attestationLevel": "attested"
    }
  ]
}
```

