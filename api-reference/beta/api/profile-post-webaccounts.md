---
title: Criar conta da
description: Criar um novo objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b1bcf743737616ac5c48d3b8c3132b57d11464ac
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812187"
---
# <a name="create-webaccount"></a><span data-ttu-id="37543-103">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="37543-103">Create webAccount</span></span>

<span data-ttu-id="37543-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37543-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37543-105">Criar um novo objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="37543-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37543-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37543-106">Permissions</span></span>

<span data-ttu-id="37543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37543-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37543-109">Permission type</span></span>                        | <span data-ttu-id="37543-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37543-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37543-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37543-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37543-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="37543-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="37543-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37543-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37543-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="37543-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="37543-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37543-115">Application</span></span>                            | <span data-ttu-id="37543-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37543-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="37543-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37543-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="37543-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37543-118">Request headers</span></span>

| <span data-ttu-id="37543-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37543-119">Name</span></span>           | <span data-ttu-id="37543-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37543-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="37543-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37543-121">Authorization</span></span>  | <span data-ttu-id="37543-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37543-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="37543-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37543-124">Content-Type</span></span>   | <span data-ttu-id="37543-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37543-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37543-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37543-127">Request body</span></span>

<span data-ttu-id="37543-128">No corpo da solicitação, forneça uma representação JSON do objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="37543-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="37543-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="37543-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="37543-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37543-130">Property</span></span>|<span data-ttu-id="37543-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37543-131">Type</span></span>|<span data-ttu-id="37543-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37543-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37543-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="37543-133">allowedAudiences</span></span>|<span data-ttu-id="37543-134">String</span><span class="sxs-lookup"><span data-stu-id="37543-134">String</span></span>|<span data-ttu-id="37543-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="37543-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="37543-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="37543-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="37543-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="37543-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="37543-138">description</span><span class="sxs-lookup"><span data-stu-id="37543-138">description</span></span>|<span data-ttu-id="37543-139">String</span><span class="sxs-lookup"><span data-stu-id="37543-139">String</span></span>|<span data-ttu-id="37543-140">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="37543-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="37543-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="37543-141">inference</span></span>|[<span data-ttu-id="37543-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="37543-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="37543-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="37543-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="37543-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="37543-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="37543-145">service</span><span class="sxs-lookup"><span data-stu-id="37543-145">service</span></span>|[<span data-ttu-id="37543-146">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="37543-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="37543-147">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="37543-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="37543-148">source</span><span class="sxs-lookup"><span data-stu-id="37543-148">source</span></span>|[<span data-ttu-id="37543-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="37543-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="37543-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="37543-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="37543-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="37543-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="37543-152">statusMessage</span><span class="sxs-lookup"><span data-stu-id="37543-152">statusMessage</span></span>|<span data-ttu-id="37543-153">String</span><span class="sxs-lookup"><span data-stu-id="37543-153">String</span></span>|<span data-ttu-id="37543-154">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="37543-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="37543-155">userId</span><span class="sxs-lookup"><span data-stu-id="37543-155">userId</span></span>|<span data-ttu-id="37543-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37543-156">String</span></span>|<span data-ttu-id="37543-157">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="37543-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="37543-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="37543-158">webUrl</span></span>|<span data-ttu-id="37543-159">String</span><span class="sxs-lookup"><span data-stu-id="37543-159">String</span></span>|<span data-ttu-id="37543-160">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="37543-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="37543-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="37543-161">Response</span></span>

<span data-ttu-id="37543-162">Se bem-sucedido, este método retorna o `201, Created` código de resposta e um novo objeto [webaccount](../resources/webaccount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37543-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37543-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37543-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37543-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37543-164">Request</span></span>

<span data-ttu-id="37543-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37543-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37543-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="37543-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37543-167">C#</span><span class="sxs-lookup"><span data-stu-id="37543-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37543-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37543-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37543-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37543-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37543-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="37543-170">Response</span></span>

<span data-ttu-id="37543-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37543-171">The following is an example of the response.</span></span>

> <span data-ttu-id="37543-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37543-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
