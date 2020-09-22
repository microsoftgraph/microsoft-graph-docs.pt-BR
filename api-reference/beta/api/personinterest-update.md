---
title: Atualizar personInterest
description: Atualize as propriedades do objeto personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 812a692a721e9d9a76cb7a0fa2547e48fb849e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067931"
---
# <a name="update-personinterest"></a><span data-ttu-id="4aa80-103">Atualizar personinterest</span><span class="sxs-lookup"><span data-stu-id="4aa80-103">Update personinterest</span></span>

<span data-ttu-id="4aa80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aa80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aa80-105">Atualiza as propriedades de um objeto [personInterest](../resources/personinterest.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4aa80-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4aa80-106">Permissions</span></span>

<span data-ttu-id="4aa80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aa80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4aa80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4aa80-109">Permission type</span></span>                        | <span data-ttu-id="4aa80-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4aa80-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4aa80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4aa80-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4aa80-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4aa80-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4aa80-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4aa80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aa80-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4aa80-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4aa80-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4aa80-115">Application</span></span>                            | <span data-ttu-id="4aa80-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aa80-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4aa80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4aa80-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
PATCH /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4aa80-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4aa80-118">Request headers</span></span>

| <span data-ttu-id="4aa80-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4aa80-119">Name</span></span>           |<span data-ttu-id="4aa80-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aa80-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4aa80-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4aa80-121">Authorization</span></span>  | <span data-ttu-id="4aa80-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4aa80-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4aa80-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aa80-124">Content-Type</span></span>   | <span data-ttu-id="4aa80-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4aa80-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aa80-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4aa80-127">Request body</span></span>

<span data-ttu-id="4aa80-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4aa80-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4aa80-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4aa80-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4aa80-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4aa80-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4aa80-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar em um objeto [personInterest](../resources/personinterest.md) existente no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4aa80-131">The following table shows the properties that are possible to update within an existing [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="4aa80-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4aa80-132">Property</span></span>|<span data-ttu-id="4aa80-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4aa80-133">Type</span></span>|<span data-ttu-id="4aa80-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aa80-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aa80-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4aa80-135">allowedAudiences</span></span>|<span data-ttu-id="4aa80-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4aa80-136">String</span></span>|<span data-ttu-id="4aa80-137">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="4aa80-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4aa80-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4aa80-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4aa80-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4aa80-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4aa80-140">categories</span><span class="sxs-lookup"><span data-stu-id="4aa80-140">categories</span></span>|<span data-ttu-id="4aa80-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4aa80-141">String collection</span></span>|<span data-ttu-id="4aa80-142">Contém categorias que um usuário associou aos juros (por exemplo, pessoal, recipies).</span><span class="sxs-lookup"><span data-stu-id="4aa80-142">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="4aa80-143">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="4aa80-143">collaborationTags</span></span>|<span data-ttu-id="4aa80-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4aa80-144">String collection</span></span>|<span data-ttu-id="4aa80-145">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="4aa80-145">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="4aa80-146">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="4aa80-146">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="4aa80-147">description</span><span class="sxs-lookup"><span data-stu-id="4aa80-147">description</span></span>|<span data-ttu-id="4aa80-148">String</span><span class="sxs-lookup"><span data-stu-id="4aa80-148">String</span></span>|<span data-ttu-id="4aa80-149">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="4aa80-149">Contains a description of the interest.</span></span>|
|<span data-ttu-id="4aa80-150">displayName</span><span class="sxs-lookup"><span data-stu-id="4aa80-150">displayName</span></span>|<span data-ttu-id="4aa80-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4aa80-151">String</span></span>|<span data-ttu-id="4aa80-152">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="4aa80-152">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="4aa80-153">fracassa</span><span class="sxs-lookup"><span data-stu-id="4aa80-153">inference</span></span>|[<span data-ttu-id="4aa80-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4aa80-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4aa80-155">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="4aa80-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4aa80-156">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4aa80-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4aa80-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="4aa80-157">webUrl</span></span>|<span data-ttu-id="4aa80-158">String</span><span class="sxs-lookup"><span data-stu-id="4aa80-158">String</span></span>|<span data-ttu-id="4aa80-159">Contém um link para uma página da Web ou recurso sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="4aa80-159">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="4aa80-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4aa80-160">Response</span></span>

<span data-ttu-id="4aa80-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personInterest](../resources/personinterest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa80-161">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4aa80-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4aa80-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4aa80-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4aa80-163">Request</span></span>

<span data-ttu-id="4aa80-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4aa80-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4aa80-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="4aa80-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "Sports"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="4aa80-166">C#</span><span class="sxs-lookup"><span data-stu-id="4aa80-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4aa80-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4aa80-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4aa80-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aa80-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4aa80-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4aa80-169">Response</span></span>

<span data-ttu-id="4aa80-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa80-170">The following is an example of the response.</span></span>

> <span data-ttu-id="4aa80-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4aa80-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


