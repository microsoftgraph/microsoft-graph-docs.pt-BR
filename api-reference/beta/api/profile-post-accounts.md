---
title: Criar conta
description: Crie um novo objeto de conta.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 308f2a1e4087fcbb07efb08be8fc1e4cba7d819f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441001"
---
# <a name="create-account"></a><span data-ttu-id="5083f-103">Criar conta</span><span class="sxs-lookup"><span data-stu-id="5083f-103">Create account</span></span>
<span data-ttu-id="5083f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5083f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5083f-105">Crie um novo [objeto userAccountInformation](../resources/useraccountinformation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5083f-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5083f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5083f-106">Permissions</span></span>

<span data-ttu-id="5083f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5083f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5083f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5083f-109">Permission type</span></span>                        | <span data-ttu-id="5083f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5083f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5083f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5083f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5083f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5083f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5083f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5083f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5083f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5083f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5083f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5083f-115">Application</span></span>                            | <span data-ttu-id="5083f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5083f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5083f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5083f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a><span data-ttu-id="5083f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5083f-118">Request headers</span></span>
|<span data-ttu-id="5083f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5083f-119">Name</span></span>|<span data-ttu-id="5083f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5083f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5083f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5083f-121">Authorization</span></span>|<span data-ttu-id="5083f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5083f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5083f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5083f-124">Content-Type</span></span>|<span data-ttu-id="5083f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5083f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5083f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5083f-127">Request body</span></span>
<span data-ttu-id="5083f-128">No corpo da solicitação, fornece uma representação JSON do [objeto userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5083f-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="5083f-129">A tabela a seguir mostra as propriedades necessárias ao criar um novo [objeto userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5083f-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="5083f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5083f-130">Property</span></span>|<span data-ttu-id="5083f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5083f-131">Type</span></span>|<span data-ttu-id="5083f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5083f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5083f-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5083f-133">allowedAudiences</span></span>|<span data-ttu-id="5083f-134">String</span><span class="sxs-lookup"><span data-stu-id="5083f-134">String</span></span>|<span data-ttu-id="5083f-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="5083f-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5083f-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5083f-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5083f-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5083f-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5083f-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="5083f-138">countryCode</span></span>|<span data-ttu-id="5083f-139">String</span><span class="sxs-lookup"><span data-stu-id="5083f-139">String</span></span>|<span data-ttu-id="5083f-140">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="5083f-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="5083f-141">inferência</span><span class="sxs-lookup"><span data-stu-id="5083f-141">inference</span></span>|[<span data-ttu-id="5083f-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5083f-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5083f-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="5083f-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5083f-144">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5083f-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5083f-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="5083f-145">preferredLanguageTag</span></span>|[<span data-ttu-id="5083f-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="5083f-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="5083f-147">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="5083f-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="5083f-148">source</span><span class="sxs-lookup"><span data-stu-id="5083f-148">source</span></span>|[<span data-ttu-id="5083f-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5083f-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5083f-150">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="5083f-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5083f-151">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5083f-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5083f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5083f-152">Response</span></span>

<span data-ttu-id="5083f-153">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5083f-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5083f-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5083f-154">Examples</span></span>


# <a name="http"></a>[<span data-ttu-id="5083f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="5083f-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/account
Content-Type: application/json
Content-length: 494

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[<span data-ttu-id="5083f-156">C#</span><span class="sxs-lookup"><span data-stu-id="5083f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-useraccountinformation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5083f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5083f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-useraccountinformation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5083f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5083f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-useraccountinformation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5083f-159">Java</span><span class="sxs-lookup"><span data-stu-id="5083f-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-useraccountinformation-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5083f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="5083f-160">Response</span></span>
<span data-ttu-id="5083f-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5083f-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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


