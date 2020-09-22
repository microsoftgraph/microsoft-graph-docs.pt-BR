---
title: Criar conta
description: Criar um novo objeto Account.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bddb2367a3f5c595fbca2609e9ec42cce7a677be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034525"
---
# <a name="create-account"></a><span data-ttu-id="57ecc-103">Criar conta</span><span class="sxs-lookup"><span data-stu-id="57ecc-103">Create account</span></span>
<span data-ttu-id="57ecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ecc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57ecc-105">Criar um novo objeto [userAccountInformation](../resources/useraccountinformation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="57ecc-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57ecc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57ecc-106">Permissions</span></span>

<span data-ttu-id="57ecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57ecc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57ecc-109">Permission type</span></span>                        | <span data-ttu-id="57ecc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57ecc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57ecc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57ecc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57ecc-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57ecc-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57ecc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57ecc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ecc-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57ecc-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57ecc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57ecc-115">Application</span></span>                            | <span data-ttu-id="57ecc-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ecc-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="57ecc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57ecc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/accounts
POST /users/{id | userPrincipalName}/profile/accounts
```

## <a name="request-headers"></a><span data-ttu-id="57ecc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ecc-118">Request headers</span></span>
|<span data-ttu-id="57ecc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="57ecc-119">Name</span></span>|<span data-ttu-id="57ecc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ecc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57ecc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="57ecc-121">Authorization</span></span>|<span data-ttu-id="57ecc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ecc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57ecc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57ecc-124">Content-Type</span></span>|<span data-ttu-id="57ecc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ecc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ecc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57ecc-127">Request body</span></span>
<span data-ttu-id="57ecc-128">No corpo da solicitação, forneça uma representação JSON do objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="57ecc-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="57ecc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um novo objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="57ecc-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="57ecc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57ecc-130">Property</span></span>|<span data-ttu-id="57ecc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57ecc-131">Type</span></span>|<span data-ttu-id="57ecc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ecc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ecc-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="57ecc-133">allowedAudiences</span></span>|<span data-ttu-id="57ecc-134">String</span><span class="sxs-lookup"><span data-stu-id="57ecc-134">String</span></span>|<span data-ttu-id="57ecc-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="57ecc-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="57ecc-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57ecc-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="57ecc-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="57ecc-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="57ecc-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="57ecc-138">countryCode</span></span>|<span data-ttu-id="57ecc-139">String</span><span class="sxs-lookup"><span data-stu-id="57ecc-139">String</span></span>|<span data-ttu-id="57ecc-140">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="57ecc-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="57ecc-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="57ecc-141">inference</span></span>|[<span data-ttu-id="57ecc-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="57ecc-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="57ecc-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="57ecc-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="57ecc-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57ecc-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="57ecc-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="57ecc-145">preferredLanguageTag</span></span>|[<span data-ttu-id="57ecc-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="57ecc-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="57ecc-147">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="57ecc-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="57ecc-148">source</span><span class="sxs-lookup"><span data-stu-id="57ecc-148">source</span></span>|[<span data-ttu-id="57ecc-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="57ecc-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="57ecc-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="57ecc-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="57ecc-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57ecc-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="57ecc-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ecc-152">Response</span></span>

<span data-ttu-id="57ecc-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57ecc-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57ecc-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57ecc-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="57ecc-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="57ecc-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/accounts
Content-Type: application/json
Content-length: 494

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[<span data-ttu-id="57ecc-156">C#</span><span class="sxs-lookup"><span data-stu-id="57ecc-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57ecc-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57ecc-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57ecc-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57ecc-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="57ecc-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ecc-159">Response</span></span>
<span data-ttu-id="57ecc-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="57ecc-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


