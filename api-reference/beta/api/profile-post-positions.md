---
title: Criar workPosition
description: Use esta API para criar um novo workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bc67994dbf3d9a6107ed2a4bcba8f0f0f090e327
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974624"
---
# <a name="create-workposition"></a><span data-ttu-id="56f57-103">Criar workPosition</span><span class="sxs-lookup"><span data-stu-id="56f57-103">Create workPosition</span></span>

<span data-ttu-id="56f57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56f57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56f57-105">Use esta API para criar um novo [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="56f57-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56f57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="56f57-106">Permissions</span></span>

<span data-ttu-id="56f57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56f57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56f57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56f57-109">Permission type</span></span>                        | <span data-ttu-id="56f57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56f57-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56f57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56f57-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56f57-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="56f57-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="56f57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56f57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56f57-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="56f57-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="56f57-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56f57-115">Application</span></span>                            | <span data-ttu-id="56f57-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f57-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="56f57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56f57-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
POST /users/{id | userPrincipalName}/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="56f57-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56f57-118">Request headers</span></span>

| <span data-ttu-id="56f57-119">Nome</span><span class="sxs-lookup"><span data-stu-id="56f57-119">Name</span></span>      |<span data-ttu-id="56f57-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56f57-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56f57-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="56f57-121">Authorization</span></span>  | <span data-ttu-id="56f57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56f57-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="56f57-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56f57-124">Content-Type</span></span>   | <span data-ttu-id="56f57-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56f57-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56f57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56f57-127">Request body</span></span>

<span data-ttu-id="56f57-128">No corpo da solicitação, forneça uma representação JSON do objeto [workPosition](../resources/workposition.md) .</span><span class="sxs-lookup"><span data-stu-id="56f57-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

<span data-ttu-id="56f57-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [workPosition](../resources/workPosition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="56f57-129">The following table shows the properties that are possible to set when you create a new [workPosition](../resources/workPosition.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="56f57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56f57-130">Property</span></span>|<span data-ttu-id="56f57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56f57-131">Type</span></span>|<span data-ttu-id="56f57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56f57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f57-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="56f57-133">allowedAudiences</span></span>|<span data-ttu-id="56f57-134">String</span><span class="sxs-lookup"><span data-stu-id="56f57-134">String</span></span>|<span data-ttu-id="56f57-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="56f57-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="56f57-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56f57-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="56f57-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="56f57-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="56f57-138">categories</span><span class="sxs-lookup"><span data-stu-id="56f57-138">categories</span></span>|<span data-ttu-id="56f57-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56f57-139">String collection</span></span>|<span data-ttu-id="56f57-140">Categorias que o usuário tenha associado a esta posição.</span><span class="sxs-lookup"><span data-stu-id="56f57-140">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="56f57-141">conhecidos</span><span class="sxs-lookup"><span data-stu-id="56f57-141">colleagues</span></span>|<span data-ttu-id="56f57-142">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="56f57-142">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="56f57-143">Colegas associados a esta posição.</span><span class="sxs-lookup"><span data-stu-id="56f57-143">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="56f57-144">detalhada</span><span class="sxs-lookup"><span data-stu-id="56f57-144">detail</span></span>|[<span data-ttu-id="56f57-145">positionDetail</span><span class="sxs-lookup"><span data-stu-id="56f57-145">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="56f57-146">Contém informações detalhadas sobre a posição.</span><span class="sxs-lookup"><span data-stu-id="56f57-146">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="56f57-147">fracassa</span><span class="sxs-lookup"><span data-stu-id="56f57-147">inference</span></span>|[<span data-ttu-id="56f57-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="56f57-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="56f57-149">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="56f57-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="56f57-150">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56f57-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="56f57-151">IsCurrent</span><span class="sxs-lookup"><span data-stu-id="56f57-151">isCurrent</span></span>|<span data-ttu-id="56f57-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="56f57-152">Boolean</span></span>|<span data-ttu-id="56f57-153">Indica se a posição é ou não atual.</span><span class="sxs-lookup"><span data-stu-id="56f57-153">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="56f57-154">manager</span><span class="sxs-lookup"><span data-stu-id="56f57-154">manager</span></span>|[<span data-ttu-id="56f57-155">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="56f57-155">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="56f57-156">Contém detalhes do gerente do usuário nesta posição.</span><span class="sxs-lookup"><span data-stu-id="56f57-156">Contains detail of the user's manager in this position.</span></span>|
|<span data-ttu-id="56f57-157">source</span><span class="sxs-lookup"><span data-stu-id="56f57-157">source</span></span>|[<span data-ttu-id="56f57-158">personDataSource</span><span class="sxs-lookup"><span data-stu-id="56f57-158">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="56f57-159">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="56f57-159">Where the values originated if synced from another service.</span></span> <span data-ttu-id="56f57-160">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56f57-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="56f57-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="56f57-161">Response</span></span>

<span data-ttu-id="56f57-162">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [workPosition](../resources/workposition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56f57-162">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56f57-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56f57-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56f57-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56f57-164">Request</span></span>

<span data-ttu-id="56f57-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56f57-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56f57-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="56f57-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/positions
Content-type: application/json

{
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting"
  },
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="56f57-167">C#</span><span class="sxs-lookup"><span data-stu-id="56f57-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workposition-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56f57-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56f57-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workposition-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56f57-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56f57-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workposition-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56f57-170">Java</span><span class="sxs-lookup"><span data-stu-id="56f57-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workposition-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56f57-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="56f57-171">Response</span></span>

<span data-ttu-id="56f57-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56f57-172">The following is an example of the response.</span></span>

> <span data-ttu-id="56f57-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56f57-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "source": null,
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```


