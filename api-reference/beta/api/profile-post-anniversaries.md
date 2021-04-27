---
title: Criar personAnniversary
description: Use essa API para criar uma nova personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c28e988290c239c8a7977df8eab6d3ae3a945372
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036965"
---
# <a name="create-personanniversary"></a><span data-ttu-id="9013e-103">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="9013e-103">Create personAnniversary</span></span>

<span data-ttu-id="9013e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9013e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9013e-105">Use essa API para criar um novo [objeto personAnniversary](../resources/personanniversary.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="9013e-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9013e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9013e-106">Permissions</span></span>

<span data-ttu-id="9013e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9013e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9013e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9013e-109">Permission type</span></span>                        | <span data-ttu-id="9013e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9013e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9013e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9013e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9013e-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9013e-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9013e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9013e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9013e-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9013e-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9013e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9013e-115">Application</span></span>                            | <span data-ttu-id="9013e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9013e-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9013e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9013e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="9013e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9013e-118">Request headers</span></span>

| <span data-ttu-id="9013e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9013e-119">Name</span></span>      |<span data-ttu-id="9013e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9013e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9013e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9013e-121">Authorization</span></span>  | <span data-ttu-id="9013e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9013e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9013e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9013e-124">Content-Type</span></span>   | <span data-ttu-id="9013e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9013e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9013e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9013e-127">Request body</span></span>

<span data-ttu-id="9013e-128">No corpo da solicitação, fornece uma representação JSON do [objeto personAnniversary.](../resources/personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="9013e-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="9013e-129">A tabela a seguir mostra as propriedades que são possíveis de definir dentro de um novo objeto \*\*personAnniversary\*\*\*\* no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="9013e-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="9013e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9013e-130">Property</span></span>|<span data-ttu-id="9013e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9013e-131">Type</span></span>|<span data-ttu-id="9013e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9013e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9013e-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="9013e-133">allowedAudiences</span></span>|<span data-ttu-id="9013e-134">String</span><span class="sxs-lookup"><span data-stu-id="9013e-134">String</span></span>|<span data-ttu-id="9013e-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="9013e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="9013e-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9013e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="9013e-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9013e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9013e-138">data</span><span class="sxs-lookup"><span data-stu-id="9013e-138">date</span></span>|<span data-ttu-id="9013e-139">Data</span><span class="sxs-lookup"><span data-stu-id="9013e-139">Date</span></span>|<span data-ttu-id="9013e-140">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="9013e-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="9013e-141">inferência</span><span class="sxs-lookup"><span data-stu-id="9013e-141">inference</span></span>|[<span data-ttu-id="9013e-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="9013e-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="9013e-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="9013e-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="9013e-144">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9013e-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9013e-145">source</span><span class="sxs-lookup"><span data-stu-id="9013e-145">source</span></span>|[<span data-ttu-id="9013e-146">personDataSource</span><span class="sxs-lookup"><span data-stu-id="9013e-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="9013e-147">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="9013e-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="9013e-148">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9013e-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9013e-149">tipo</span><span class="sxs-lookup"><span data-stu-id="9013e-149">type</span></span>|<span data-ttu-id="9013e-150">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="9013e-150">anniversaryType</span></span>|<span data-ttu-id="9013e-151">O tipo de aniversário que a data representa.</span><span class="sxs-lookup"><span data-stu-id="9013e-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="9013e-152">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9013e-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="9013e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9013e-153">Response</span></span>

<span data-ttu-id="9013e-154">Se tiver êxito, este método retornará `201, Created` o código de resposta e um novo objeto [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9013e-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9013e-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9013e-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9013e-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9013e-156">Request</span></span>

<span data-ttu-id="9013e-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9013e-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9013e-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9013e-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "birthday",
  "date": "1980-01-08"
}
```
# <a name="c"></a>[<span data-ttu-id="9013e-159">C#</span><span class="sxs-lookup"><span data-stu-id="9013e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9013e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9013e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9013e-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9013e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9013e-162">Java</span><span class="sxs-lookup"><span data-stu-id="9013e-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personanniversary-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9013e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9013e-163">Response</span></span>

<span data-ttu-id="9013e-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9013e-164">The following is an example of the response.</span></span>

> <span data-ttu-id="9013e-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9013e-165">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
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
  "type": "birthday",
  "date": "Date"
}
```


