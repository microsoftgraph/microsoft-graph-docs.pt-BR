---
title: Atualizar webaccount
description: Atualizar as propriedades de um objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6df75e05761d47e513272a222e956ee64235bde3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973947"
---
# <a name="update-webaccount"></a><span data-ttu-id="04576-103">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="04576-103">Update webAccount</span></span>

<span data-ttu-id="04576-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04576-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04576-105">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="04576-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04576-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04576-106">Permissions</span></span>

<span data-ttu-id="04576-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04576-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04576-109">Permission type</span></span>                        | <span data-ttu-id="04576-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04576-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04576-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04576-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04576-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="04576-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="04576-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04576-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04576-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="04576-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="04576-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04576-115">Application</span></span>                            | <span data-ttu-id="04576-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04576-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="04576-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04576-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
PATCH /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04576-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04576-118">Request headers</span></span>

| <span data-ttu-id="04576-119">Nome</span><span class="sxs-lookup"><span data-stu-id="04576-119">Name</span></span>           |<span data-ttu-id="04576-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="04576-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="04576-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04576-121">Authorization</span></span>  | <span data-ttu-id="04576-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04576-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="04576-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04576-124">Content-Type</span></span>   | <span data-ttu-id="04576-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04576-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="04576-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04576-127">Request body</span></span>

<span data-ttu-id="04576-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="04576-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="04576-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="04576-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="04576-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="04576-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="04576-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04576-131">Property</span></span>|<span data-ttu-id="04576-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="04576-132">Type</span></span>|<span data-ttu-id="04576-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="04576-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04576-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="04576-134">allowedAudiences</span></span>|<span data-ttu-id="04576-135">String</span><span class="sxs-lookup"><span data-stu-id="04576-135">String</span></span>|<span data-ttu-id="04576-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="04576-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="04576-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="04576-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="04576-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="04576-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="04576-139">description</span><span class="sxs-lookup"><span data-stu-id="04576-139">description</span></span>|<span data-ttu-id="04576-140">String</span><span class="sxs-lookup"><span data-stu-id="04576-140">String</span></span>|<span data-ttu-id="04576-141">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="04576-141">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="04576-142">fracassa</span><span class="sxs-lookup"><span data-stu-id="04576-142">inference</span></span>|[<span data-ttu-id="04576-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="04576-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="04576-144">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="04576-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="04576-145">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="04576-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="04576-146">serviço</span><span class="sxs-lookup"><span data-stu-id="04576-146">service</span></span>|[<span data-ttu-id="04576-147">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="04576-147">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="04576-148">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="04576-148">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="04576-149">statusMessage</span><span class="sxs-lookup"><span data-stu-id="04576-149">statusMessage</span></span>|<span data-ttu-id="04576-150">String</span><span class="sxs-lookup"><span data-stu-id="04576-150">String</span></span>|<span data-ttu-id="04576-151">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="04576-151">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="04576-152">userId</span><span class="sxs-lookup"><span data-stu-id="04576-152">userId</span></span>|<span data-ttu-id="04576-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04576-153">String</span></span>|<span data-ttu-id="04576-154">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="04576-154">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="04576-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="04576-155">webUrl</span></span>|<span data-ttu-id="04576-156">String</span><span class="sxs-lookup"><span data-stu-id="04576-156">String</span></span>|<span data-ttu-id="04576-157">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="04576-157">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="04576-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="04576-158">Response</span></span>

<span data-ttu-id="04576-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [webaccount](../resources/webaccount.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04576-159">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04576-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04576-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04576-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04576-161">Request</span></span>

<span data-ttu-id="04576-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04576-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04576-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="04576-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "webUrl": "https://github.com/innocenty.popov"
}
```
# <a name="c"></a>[<span data-ttu-id="04576-164">C#</span><span class="sxs-lookup"><span data-stu-id="04576-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04576-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04576-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04576-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04576-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04576-167">Java</span><span class="sxs-lookup"><span data-stu-id="04576-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-webaccount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04576-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="04576-168">Response</span></span>

<span data-ttu-id="04576-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04576-169">The following is an example of the response.</span></span>

> <span data-ttu-id="04576-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04576-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
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


