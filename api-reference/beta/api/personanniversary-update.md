---
title: Atualizar personAnniversary
description: Atualize as propriedades do objeto personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2951ccaf9368aec3bc28fdf6ab278437f5b9d18d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968425"
---
# <a name="update-personanniversary"></a><span data-ttu-id="65b96-103">Atualizar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="65b96-103">Update personAnniversary</span></span>

<span data-ttu-id="65b96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b96-105">Atualiza as propriedades de um objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="65b96-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65b96-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65b96-106">Permissions</span></span>

<span data-ttu-id="65b96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65b96-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65b96-109">Permission type</span></span>                        | <span data-ttu-id="65b96-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65b96-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65b96-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65b96-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65b96-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="65b96-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65b96-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65b96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b96-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="65b96-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65b96-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65b96-115">Application</span></span>                            | <span data-ttu-id="65b96-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b96-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="65b96-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65b96-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id}
PATCH /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65b96-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65b96-118">Request headers</span></span>

| <span data-ttu-id="65b96-119">Nome</span><span class="sxs-lookup"><span data-stu-id="65b96-119">Name</span></span>           |<span data-ttu-id="65b96-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="65b96-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="65b96-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="65b96-121">Authorization</span></span>  | <span data-ttu-id="65b96-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65b96-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="65b96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65b96-124">Content-Type</span></span>   | <span data-ttu-id="65b96-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65b96-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65b96-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65b96-127">Request body</span></span>

<span data-ttu-id="65b96-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="65b96-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="65b96-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="65b96-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="65b96-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="65b96-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="65b96-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar em um objeto [personAnniversary](../resources/personanniversary.md) existente no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="65b96-131">The following table shows the properties that are possible to update within an existing [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="65b96-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65b96-132">Property</span></span>|<span data-ttu-id="65b96-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="65b96-133">Type</span></span>|<span data-ttu-id="65b96-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="65b96-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b96-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="65b96-135">allowedAudiences</span></span>|<span data-ttu-id="65b96-136">String</span><span class="sxs-lookup"><span data-stu-id="65b96-136">String</span></span>|<span data-ttu-id="65b96-137">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="65b96-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="65b96-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="65b96-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="65b96-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="65b96-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="65b96-140">data</span><span class="sxs-lookup"><span data-stu-id="65b96-140">date</span></span>|<span data-ttu-id="65b96-141">Data</span><span class="sxs-lookup"><span data-stu-id="65b96-141">Date</span></span>|<span data-ttu-id="65b96-142">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="65b96-142">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="65b96-143">fracassa</span><span class="sxs-lookup"><span data-stu-id="65b96-143">inference</span></span>|[<span data-ttu-id="65b96-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="65b96-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="65b96-145">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="65b96-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="65b96-146">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="65b96-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="65b96-147">tipo</span><span class="sxs-lookup"><span data-stu-id="65b96-147">type</span></span>|<span data-ttu-id="65b96-148">data especial</span><span class="sxs-lookup"><span data-stu-id="65b96-148">anniversaryType</span></span>|<span data-ttu-id="65b96-149">O tipo de aniversário que a data representa.</span><span class="sxs-lookup"><span data-stu-id="65b96-149">The type of anniversary the date represents.</span></span> <span data-ttu-id="65b96-150">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="65b96-150">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="65b96-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b96-151">Response</span></span>

<span data-ttu-id="65b96-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personAnniversary](../resources/personanniversary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65b96-152">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65b96-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65b96-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65b96-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65b96-154">Request</span></span>

<span data-ttu-id="65b96-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65b96-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65b96-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b96-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "allowedAudiences": "contacts"
}
```
# <a name="c"></a>[<span data-ttu-id="65b96-157">C#</span><span class="sxs-lookup"><span data-stu-id="65b96-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65b96-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b96-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b96-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b96-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65b96-160">Java</span><span class="sxs-lookup"><span data-stu-id="65b96-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personanniversary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="65b96-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b96-161">Response</span></span>

<span data-ttu-id="65b96-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65b96-162">The following is an example of the response.</span></span>

> <span data-ttu-id="65b96-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65b96-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "contacts",
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


