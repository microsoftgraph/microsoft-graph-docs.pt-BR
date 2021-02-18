---
title: Atualizar userAccountInformation
description: Atualizar as propriedades do objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8638eeadd59ba7efaae0e6ad32bd4f740dab6d36
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291976"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="1308b-103">Atualizar useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="1308b-103">Update useraccountinformation</span></span>

<span data-ttu-id="1308b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1308b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1308b-105">Atualizar as propriedades de um [objeto userAccountInformation](../resources/useraccountinformation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="1308b-105">Update the properties of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1308b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1308b-106">Permissions</span></span>

<span data-ttu-id="1308b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1308b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1308b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1308b-109">Permission type</span></span>                        | <span data-ttu-id="1308b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1308b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1308b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1308b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1308b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1308b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1308b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1308b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1308b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1308b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1308b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1308b-115">Application</span></span>                            | <span data-ttu-id="1308b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1308b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1308b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1308b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
PATCH /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1308b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1308b-118">Request headers</span></span>

| <span data-ttu-id="1308b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1308b-119">Name</span></span>           |<span data-ttu-id="1308b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1308b-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="1308b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1308b-121">Authorization</span></span>  | <span data-ttu-id="1308b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1308b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1308b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1308b-124">Content-Type</span></span>   | <span data-ttu-id="1308b-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="1308b-125">application/json.</span></span> <span data-ttu-id="1308b-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="1308b-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="1308b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1308b-127">Request body</span></span>

<span data-ttu-id="1308b-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1308b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1308b-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1308b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1308b-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1308b-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="1308b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1308b-131">Property</span></span>|<span data-ttu-id="1308b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1308b-132">Type</span></span>|<span data-ttu-id="1308b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1308b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1308b-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1308b-134">allowedAudiences</span></span>|<span data-ttu-id="1308b-135">String</span><span class="sxs-lookup"><span data-stu-id="1308b-135">String</span></span>|<span data-ttu-id="1308b-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="1308b-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1308b-137">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1308b-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1308b-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1308b-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1308b-139">countryCode</span><span class="sxs-lookup"><span data-stu-id="1308b-139">countryCode</span></span>|<span data-ttu-id="1308b-140">String</span><span class="sxs-lookup"><span data-stu-id="1308b-140">String</span></span>|<span data-ttu-id="1308b-141">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="1308b-141">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="1308b-142">inferência</span><span class="sxs-lookup"><span data-stu-id="1308b-142">inference</span></span>|[<span data-ttu-id="1308b-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1308b-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1308b-144">Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1308b-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1308b-145">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1308b-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1308b-146">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="1308b-146">preferredLanguageTag</span></span>|[<span data-ttu-id="1308b-147">localeInfo</span><span class="sxs-lookup"><span data-stu-id="1308b-147">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="1308b-148">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="1308b-148">Contains the language the user has associated as preferred for the account.</span></span>   |

## <a name="response"></a><span data-ttu-id="1308b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1308b-149">Response</span></span>

<span data-ttu-id="1308b-150">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [userAccountInformation](../resources/useraccountinformation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1308b-150">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1308b-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1308b-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1308b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1308b-152">Request</span></span>

<span data-ttu-id="1308b-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1308b-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1308b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1308b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "countryCode": "NO"
}
```
# <a name="c"></a>[<span data-ttu-id="1308b-155">C#</span><span class="sxs-lookup"><span data-stu-id="1308b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1308b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1308b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1308b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1308b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1308b-158">Java</span><span class="sxs-lookup"><span data-stu-id="1308b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1308b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1308b-159">Response</span></span>

<span data-ttu-id="1308b-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1308b-160">The following is an example of the response.</span></span>

> <span data-ttu-id="1308b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1308b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


