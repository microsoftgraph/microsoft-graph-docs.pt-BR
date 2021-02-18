---
title: Criar conta
description: Criar um novo objeto de conta.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d1fb13f513450515361f2bdb15ebfd7461635e1c
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292970"
---
# <a name="create-account"></a><span data-ttu-id="48635-103">Criar conta</span><span class="sxs-lookup"><span data-stu-id="48635-103">Create account</span></span>
<span data-ttu-id="48635-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48635-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48635-105">Crie um novo [objeto userAccountInformation](../resources/useraccountinformation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="48635-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48635-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="48635-106">Permissions</span></span>

<span data-ttu-id="48635-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48635-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48635-109">Permission type</span></span>                        | <span data-ttu-id="48635-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48635-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48635-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48635-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48635-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48635-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="48635-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48635-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48635-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48635-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="48635-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48635-115">Application</span></span>                            | <span data-ttu-id="48635-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48635-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="48635-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48635-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a><span data-ttu-id="48635-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48635-118">Request headers</span></span>
|<span data-ttu-id="48635-119">Nome</span><span class="sxs-lookup"><span data-stu-id="48635-119">Name</span></span>|<span data-ttu-id="48635-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="48635-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48635-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="48635-121">Authorization</span></span>|<span data-ttu-id="48635-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48635-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="48635-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48635-124">Content-Type</span></span>|<span data-ttu-id="48635-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48635-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48635-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48635-127">Request body</span></span>
<span data-ttu-id="48635-128">No corpo da solicitação, fornece uma representação JSON do [objeto userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="48635-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="48635-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um novo [objeto userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="48635-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="48635-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48635-130">Property</span></span>|<span data-ttu-id="48635-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="48635-131">Type</span></span>|<span data-ttu-id="48635-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48635-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48635-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="48635-133">allowedAudiences</span></span>|<span data-ttu-id="48635-134">String</span><span class="sxs-lookup"><span data-stu-id="48635-134">String</span></span>|<span data-ttu-id="48635-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="48635-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="48635-136">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="48635-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="48635-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="48635-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="48635-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="48635-138">countryCode</span></span>|<span data-ttu-id="48635-139">String</span><span class="sxs-lookup"><span data-stu-id="48635-139">String</span></span>|<span data-ttu-id="48635-140">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="48635-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="48635-141">inferência</span><span class="sxs-lookup"><span data-stu-id="48635-141">inference</span></span>|[<span data-ttu-id="48635-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="48635-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="48635-143">Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48635-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="48635-144">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="48635-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="48635-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="48635-145">preferredLanguageTag</span></span>|[<span data-ttu-id="48635-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="48635-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="48635-147">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="48635-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="48635-148">source</span><span class="sxs-lookup"><span data-stu-id="48635-148">source</span></span>|[<span data-ttu-id="48635-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="48635-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="48635-150">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="48635-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="48635-151">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="48635-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="48635-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="48635-152">Response</span></span>

<span data-ttu-id="48635-153">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48635-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48635-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48635-154">Examples</span></span>

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

### <a name="response"></a><span data-ttu-id="48635-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="48635-155">Response</span></span>
<span data-ttu-id="48635-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48635-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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


