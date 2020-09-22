---
title: Atualizar personWebsite
description: Atualiza as propriedades de um objeto personWebsite no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 33b99ded6830a3e9ed4cd985be760824f18e8ee6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010651"
---
# <a name="update-personwebsite"></a><span data-ttu-id="d2ef8-103">Atualizar personwebsite</span><span class="sxs-lookup"><span data-stu-id="d2ef8-103">Update personwebsite</span></span>

<span data-ttu-id="d2ef8-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d2ef8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2ef8-105">Atualiza as propriedades do objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2ef8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2ef8-106">Permissions</span></span>

<span data-ttu-id="d2ef8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2ef8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2ef8-109">Permission type</span></span>                        | <span data-ttu-id="d2ef8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2ef8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2ef8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2ef8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2ef8-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2ef8-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d2ef8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2ef8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ef8-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2ef8-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d2ef8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2ef8-115">Application</span></span>                            | <span data-ttu-id="d2ef8-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ef8-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d2ef8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2ef8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
PATCH /users/{id | userPrincipalName}/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2ef8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ef8-118">Request headers</span></span>

| <span data-ttu-id="d2ef8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d2ef8-119">Name</span></span>           |<span data-ttu-id="d2ef8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ef8-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d2ef8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2ef8-121">Authorization</span></span>  | <span data-ttu-id="d2ef8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d2ef8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2ef8-124">Content-Type</span></span>   | <span data-ttu-id="d2ef8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2ef8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ef8-127">Request body</span></span>

<span data-ttu-id="d2ef8-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d2ef8-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d2ef8-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d2ef8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2ef8-131">Property</span></span>|<span data-ttu-id="d2ef8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2ef8-132">Type</span></span>|<span data-ttu-id="d2ef8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ef8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ef8-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d2ef8-134">allowedAudiences</span></span>|<span data-ttu-id="d2ef8-135">String</span><span class="sxs-lookup"><span data-stu-id="d2ef8-135">String</span></span>|<span data-ttu-id="d2ef8-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d2ef8-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d2ef8-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d2ef8-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d2ef8-139">Categorias</span><span class="sxs-lookup"><span data-stu-id="d2ef8-139">categories</span></span>|<span data-ttu-id="d2ef8-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2ef8-140">String collection</span></span>|<span data-ttu-id="d2ef8-141">Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).</span><span class="sxs-lookup"><span data-stu-id="d2ef8-141">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="d2ef8-142">description</span><span class="sxs-lookup"><span data-stu-id="d2ef8-142">description</span></span>|<span data-ttu-id="d2ef8-143">String</span><span class="sxs-lookup"><span data-stu-id="d2ef8-143">String</span></span>|<span data-ttu-id="d2ef8-144">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-144">Contains a description of the website.</span></span>|
|<span data-ttu-id="d2ef8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d2ef8-145">displayName</span></span>|<span data-ttu-id="d2ef8-146">String</span><span class="sxs-lookup"><span data-stu-id="d2ef8-146">String</span></span>|<span data-ttu-id="d2ef8-147">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-147">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="d2ef8-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="d2ef8-148">inference</span></span>|[<span data-ttu-id="d2ef8-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d2ef8-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d2ef8-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d2ef8-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d2ef8-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2ef8-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="d2ef8-152">webUrl</span></span>|<span data-ttu-id="d2ef8-153">String</span><span class="sxs-lookup"><span data-stu-id="d2ef8-153">String</span></span>|<span data-ttu-id="d2ef8-154">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-154">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="d2ef8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2ef8-155">Response</span></span>

<span data-ttu-id="d2ef8-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personWebsite](../resources/personwebsite.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-156">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2ef8-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2ef8-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2ef8-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ef8-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="d2ef8-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2ef8-159">HTTP</span></span>](#tab/http)

<span data-ttu-id="d2ef8-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-160">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/websites/{id}
Content-type: application/json

{
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}
```
# <a name="c"></a>[<span data-ttu-id="d2ef8-161">C#</span><span class="sxs-lookup"><span data-stu-id="d2ef8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2ef8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2ef8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2ef8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2ef8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d2ef8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2ef8-164">Response</span></span>

<span data-ttu-id="d2ef8-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-165">The following is an example of the response.</span></span>

> <span data-ttu-id="d2ef8-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2ef8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
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
  "categories": [
    "football"
  ],
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


