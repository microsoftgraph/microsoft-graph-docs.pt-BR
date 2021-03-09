---
title: Atualizar itememail
description: Atualize as propriedades de um objeto itemEmail no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e37adabbb0fc9ce8e355d2ab6e8d6a302fe14918
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577491"
---
# <a name="update-itememail"></a><span data-ttu-id="cbaab-103">Atualizar itememail</span><span class="sxs-lookup"><span data-stu-id="cbaab-103">Update itememail</span></span>

<span data-ttu-id="cbaab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbaab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbaab-105">Atualize as propriedades de [um objeto itemEmail](../resources/itememail.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="cbaab-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cbaab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbaab-106">Permissions</span></span>

<span data-ttu-id="cbaab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbaab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbaab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbaab-109">Permission type</span></span>                        | <span data-ttu-id="cbaab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbaab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cbaab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbaab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbaab-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbaab-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cbaab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbaab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbaab-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbaab-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cbaab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbaab-115">Application</span></span>                            | <span data-ttu-id="cbaab-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbaab-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="cbaab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbaab-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/emails/{id}
PATCH /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cbaab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaab-118">Request headers</span></span>
|<span data-ttu-id="cbaab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cbaab-119">Name</span></span>|<span data-ttu-id="cbaab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbaab-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cbaab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbaab-121">Authorization</span></span>|<span data-ttu-id="cbaab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbaab-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cbaab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbaab-124">Content-Type</span></span>|<span data-ttu-id="cbaab-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbaab-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbaab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaab-127">Request body</span></span>

<span data-ttu-id="cbaab-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="cbaab-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cbaab-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="cbaab-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cbaab-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cbaab-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="cbaab-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar dentro de um [objeto itemEmail](../resources/itememail.md) existente no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="cbaab-131">The following table shows the properties that are possible to update within an existing [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="cbaab-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbaab-132">Property</span></span>|<span data-ttu-id="cbaab-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbaab-133">Type</span></span>|<span data-ttu-id="cbaab-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbaab-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbaab-135">address</span><span class="sxs-lookup"><span data-stu-id="cbaab-135">address</span></span>|<span data-ttu-id="cbaab-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbaab-136">String</span></span>|<span data-ttu-id="cbaab-137">O endereço de email em si.</span><span class="sxs-lookup"><span data-stu-id="cbaab-137">The email address itself.</span></span>|
|<span data-ttu-id="cbaab-138">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="cbaab-138">allowedAudiences</span></span>|<span data-ttu-id="cbaab-139">String</span><span class="sxs-lookup"><span data-stu-id="cbaab-139">String</span></span>|<span data-ttu-id="cbaab-140">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="cbaab-140">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="cbaab-141">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cbaab-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="cbaab-142">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cbaab-142">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cbaab-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cbaab-143">displayName</span></span>|<span data-ttu-id="cbaab-144">String</span><span class="sxs-lookup"><span data-stu-id="cbaab-144">String</span></span>|<span data-ttu-id="cbaab-145">O nome ou o rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="cbaab-145">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="cbaab-146">inferência</span><span class="sxs-lookup"><span data-stu-id="cbaab-146">inference</span></span>|[<span data-ttu-id="cbaab-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="cbaab-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="cbaab-148">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="cbaab-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="cbaab-149">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cbaab-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cbaab-150">source</span><span class="sxs-lookup"><span data-stu-id="cbaab-150">source</span></span>|[<span data-ttu-id="cbaab-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="cbaab-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="cbaab-152">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="cbaab-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="cbaab-153">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cbaab-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cbaab-154">tipo</span><span class="sxs-lookup"><span data-stu-id="cbaab-154">type</span></span>|<span data-ttu-id="cbaab-155">emailType</span><span class="sxs-lookup"><span data-stu-id="cbaab-155">emailType</span></span>|<span data-ttu-id="cbaab-156">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="cbaab-156">The type of email address.</span></span> <span data-ttu-id="cbaab-157">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="cbaab-157">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="cbaab-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbaab-158">Response</span></span>

<span data-ttu-id="cbaab-159">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto itemEmail](../resources/itememail.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbaab-159">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cbaab-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cbaab-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cbaab-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaab-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="cbaab-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbaab-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/emails/{id}
Content-Type: application/json
Content-length: 383

{
  "displayName": "Business Email",
  "type": "work"
}
```
# <a name="c"></a>[<span data-ttu-id="cbaab-163">C#</span><span class="sxs-lookup"><span data-stu-id="cbaab-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbaab-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbaab-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbaab-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbaab-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cbaab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbaab-166">Response</span></span>
<span data-ttu-id="cbaab-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbaab-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
}
-->
``` http
HTTP/1.1 200 OK
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": "Business Email",
  "type": "work"
}
```


