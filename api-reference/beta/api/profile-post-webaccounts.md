---
title: Criar conta da
description: Criar um novo objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 697791bff68443cedd3e094c8ae2d3706ab2b072
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972645"
---
# <a name="create-webaccount"></a><span data-ttu-id="9e767-103">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="9e767-103">Create webAccount</span></span>

<span data-ttu-id="9e767-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e767-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e767-105">Criar um novo objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9e767-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e767-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e767-106">Permissions</span></span>

<span data-ttu-id="9e767-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e767-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e767-109">Permission type</span></span>                        | <span data-ttu-id="9e767-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e767-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e767-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e767-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e767-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e767-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9e767-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e767-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e767-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e767-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9e767-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e767-115">Application</span></span>                            | <span data-ttu-id="9e767-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e767-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9e767-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e767-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="9e767-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e767-118">Request headers</span></span>

| <span data-ttu-id="9e767-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9e767-119">Name</span></span>           | <span data-ttu-id="9e767-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e767-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="9e767-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e767-121">Authorization</span></span>  | <span data-ttu-id="9e767-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e767-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9e767-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e767-124">Content-Type</span></span>   | <span data-ttu-id="9e767-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e767-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e767-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e767-127">Request body</span></span>

<span data-ttu-id="9e767-128">No corpo da solicitação, forneça uma representação JSON do objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="9e767-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="9e767-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9e767-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="9e767-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e767-130">Property</span></span>|<span data-ttu-id="9e767-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e767-131">Type</span></span>|<span data-ttu-id="9e767-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e767-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e767-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="9e767-133">allowedAudiences</span></span>|<span data-ttu-id="9e767-134">String</span><span class="sxs-lookup"><span data-stu-id="9e767-134">String</span></span>|<span data-ttu-id="9e767-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="9e767-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="9e767-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9e767-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="9e767-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e767-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9e767-138">description</span><span class="sxs-lookup"><span data-stu-id="9e767-138">description</span></span>|<span data-ttu-id="9e767-139">String</span><span class="sxs-lookup"><span data-stu-id="9e767-139">String</span></span>|<span data-ttu-id="9e767-140">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="9e767-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="9e767-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="9e767-141">inference</span></span>|[<span data-ttu-id="9e767-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="9e767-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="9e767-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="9e767-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="9e767-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9e767-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9e767-145">serviço</span><span class="sxs-lookup"><span data-stu-id="9e767-145">service</span></span>|[<span data-ttu-id="9e767-146">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="9e767-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="9e767-147">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="9e767-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="9e767-148">source</span><span class="sxs-lookup"><span data-stu-id="9e767-148">source</span></span>|[<span data-ttu-id="9e767-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="9e767-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="9e767-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="9e767-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="9e767-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9e767-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9e767-152">statusMessage</span><span class="sxs-lookup"><span data-stu-id="9e767-152">statusMessage</span></span>|<span data-ttu-id="9e767-153">String</span><span class="sxs-lookup"><span data-stu-id="9e767-153">String</span></span>|<span data-ttu-id="9e767-154">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="9e767-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="9e767-155">userId</span><span class="sxs-lookup"><span data-stu-id="9e767-155">userId</span></span>|<span data-ttu-id="9e767-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e767-156">String</span></span>|<span data-ttu-id="9e767-157">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="9e767-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="9e767-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="9e767-158">webUrl</span></span>|<span data-ttu-id="9e767-159">String</span><span class="sxs-lookup"><span data-stu-id="9e767-159">String</span></span>|<span data-ttu-id="9e767-160">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="9e767-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="9e767-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e767-161">Response</span></span>

<span data-ttu-id="9e767-162">Se bem-sucedido, este método retorna o `201, Created` código de resposta e um novo objeto [webaccount](../resources/webaccount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e767-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e767-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e767-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e767-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e767-164">Request</span></span>

<span data-ttu-id="9e767-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e767-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e767-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e767-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9e767-167">C#</span><span class="sxs-lookup"><span data-stu-id="9e767-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e767-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e767-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e767-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e767-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e767-170">Java</span><span class="sxs-lookup"><span data-stu-id="9e767-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-webaccount-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e767-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e767-171">Response</span></span>

<span data-ttu-id="9e767-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e767-172">The following is an example of the response.</span></span>

> <span data-ttu-id="9e767-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e767-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  },
  "statusMessage": null,
  "webUrl": "https://github.com/innocenty.popov"
}
```


