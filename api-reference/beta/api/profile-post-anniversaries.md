---
title: Criar personAnniversary
description: Use esta API para criar um novo personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 92caed6f034b53c53d21f6a0931b3f9e4786e26a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810066"
---
# <a name="create-personanniversary"></a><span data-ttu-id="db42c-103">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="db42c-103">Create personAnniversary</span></span>

<span data-ttu-id="db42c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db42c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db42c-105">Use esta API para criar um novo objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="db42c-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db42c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db42c-106">Permissions</span></span>

<span data-ttu-id="db42c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db42c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db42c-109">Permission type</span></span>                        | <span data-ttu-id="db42c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db42c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db42c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db42c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db42c-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="db42c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="db42c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db42c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db42c-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="db42c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="db42c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db42c-115">Application</span></span>                            | <span data-ttu-id="db42c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db42c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="db42c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db42c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="db42c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db42c-118">Request headers</span></span>

| <span data-ttu-id="db42c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="db42c-119">Name</span></span>      |<span data-ttu-id="db42c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="db42c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db42c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="db42c-121">Authorization</span></span>  | <span data-ttu-id="db42c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db42c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="db42c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db42c-124">Content-Type</span></span>   | <span data-ttu-id="db42c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db42c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db42c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db42c-127">Request body</span></span>

<span data-ttu-id="db42c-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAnniversary](../resources/personanniversary.md) .</span><span class="sxs-lookup"><span data-stu-id="db42c-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="db42c-129">A tabela a seguir mostra as propriedades que podem ser definidas em um novo objeto \* \* personAnniversary \* \*, no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="db42c-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="db42c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db42c-130">Property</span></span>|<span data-ttu-id="db42c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db42c-131">Type</span></span>|<span data-ttu-id="db42c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db42c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db42c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="db42c-133">allowedAudiences</span></span>|<span data-ttu-id="db42c-134">String</span><span class="sxs-lookup"><span data-stu-id="db42c-134">String</span></span>|<span data-ttu-id="db42c-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="db42c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="db42c-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="db42c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="db42c-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="db42c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="db42c-138">data</span><span class="sxs-lookup"><span data-stu-id="db42c-138">date</span></span>|<span data-ttu-id="db42c-139">Data</span><span class="sxs-lookup"><span data-stu-id="db42c-139">Date</span></span>|<span data-ttu-id="db42c-140">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="db42c-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="db42c-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="db42c-141">inference</span></span>|[<span data-ttu-id="db42c-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="db42c-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="db42c-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="db42c-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="db42c-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="db42c-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="db42c-145">source</span><span class="sxs-lookup"><span data-stu-id="db42c-145">source</span></span>|[<span data-ttu-id="db42c-146">personDataSource</span><span class="sxs-lookup"><span data-stu-id="db42c-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="db42c-147">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="db42c-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="db42c-148">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="db42c-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="db42c-149">type</span><span class="sxs-lookup"><span data-stu-id="db42c-149">type</span></span>|<span data-ttu-id="db42c-150">data especial</span><span class="sxs-lookup"><span data-stu-id="db42c-150">anniversaryType</span></span>|<span data-ttu-id="db42c-151">O tipo de aniversário que a data representa.</span><span class="sxs-lookup"><span data-stu-id="db42c-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="db42c-152">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="db42c-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="db42c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="db42c-153">Response</span></span>

<span data-ttu-id="db42c-154">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db42c-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db42c-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db42c-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db42c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db42c-156">Request</span></span>

<span data-ttu-id="db42c-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db42c-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db42c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="db42c-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="db42c-159">C#</span><span class="sxs-lookup"><span data-stu-id="db42c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db42c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db42c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db42c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db42c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="db42c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="db42c-162">Response</span></span>

<span data-ttu-id="db42c-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db42c-163">The following is an example of the response.</span></span>

> <span data-ttu-id="db42c-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db42c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
