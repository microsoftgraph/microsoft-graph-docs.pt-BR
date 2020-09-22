---
title: Criar skillProficiency
description: Use esta API para criar um novo skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a13713904da19cc4b13729633e63e81275596833
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034354"
---
# <a name="create-skillproficiency"></a><span data-ttu-id="1ea9d-103">Criar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="1ea9d-103">Create skillProficiency</span></span>

<span data-ttu-id="1ea9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ea9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ea9d-105">Use esta API para criar um novo objeto [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-105">Use this API to create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ea9d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ea9d-106">Permissions</span></span>

<span data-ttu-id="1ea9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ea9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ea9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ea9d-109">Permission type</span></span>                        | <span data-ttu-id="1ea9d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ea9d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ea9d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ea9d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ea9d-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1ea9d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1ea9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ea9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ea9d-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1ea9d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1ea9d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ea9d-115">Application</span></span>                            | <span data-ttu-id="1ea9d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ea9d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1ea9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ea9d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
POST /users/{id | userPrincipalName}/profile/skills
```

## <a name="request-headers"></a><span data-ttu-id="1ea9d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea9d-118">Request headers</span></span>

| <span data-ttu-id="1ea9d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1ea9d-119">Name</span></span>           | <span data-ttu-id="1ea9d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea9d-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="1ea9d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ea9d-121">Authorization</span></span>  | <span data-ttu-id="1ea9d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1ea9d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ea9d-124">Content-Type</span></span>   | <span data-ttu-id="1ea9d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ea9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea9d-127">Request body</span></span>

<span data-ttu-id="1ea9d-128">No corpo da solicitação, forneça uma representação JSON do objeto [skillProficiency](../resources/skillproficiency.md) .</span><span class="sxs-lookup"><span data-stu-id="1ea9d-128">In the request body, supply a JSON representation of [skillProficiency](../resources/skillproficiency.md) object.</span></span>

<span data-ttu-id="1ea9d-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-129">The following table shows the properties that are possible to set when you create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="1ea9d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ea9d-130">Property</span></span>|<span data-ttu-id="1ea9d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ea9d-131">Type</span></span>|<span data-ttu-id="1ea9d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea9d-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1ea9d-133">allowedAudiences</span></span>|<span data-ttu-id="1ea9d-134">String</span><span class="sxs-lookup"><span data-stu-id="1ea9d-134">String</span></span>|<span data-ttu-id="1ea9d-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1ea9d-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ea9d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1ea9d-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1ea9d-138">categories</span><span class="sxs-lookup"><span data-stu-id="1ea9d-138">categories</span></span>|<span data-ttu-id="1ea9d-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ea9d-139">String collection</span></span>|<span data-ttu-id="1ea9d-140">Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby).</span><span class="sxs-lookup"><span data-stu-id="1ea9d-140">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="1ea9d-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="1ea9d-141">collaborationTags</span></span>|<span data-ttu-id="1ea9d-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1ea9d-142">String collection</span></span>|<span data-ttu-id="1ea9d-143">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="1ea9d-144">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="1ea9d-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="1ea9d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1ea9d-145">displayName</span></span>|<span data-ttu-id="1ea9d-146">String</span><span class="sxs-lookup"><span data-stu-id="1ea9d-146">String</span></span>|<span data-ttu-id="1ea9d-147">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-147">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="1ea9d-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="1ea9d-148">inference</span></span>|[<span data-ttu-id="1ea9d-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1ea9d-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1ea9d-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1ea9d-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ea9d-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1ea9d-152">proficiência</span><span class="sxs-lookup"><span data-stu-id="1ea9d-152">proficiency</span></span>|<span data-ttu-id="1ea9d-153">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="1ea9d-153">skillProficiencyLevel</span></span>|<span data-ttu-id="1ea9d-154">Detalhes da proficiência dos usuários com esta habilidade.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-154">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="1ea9d-155">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-155">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1ea9d-156">source</span><span class="sxs-lookup"><span data-stu-id="1ea9d-156">source</span></span>|[<span data-ttu-id="1ea9d-157">personDataSource</span><span class="sxs-lookup"><span data-stu-id="1ea9d-157">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1ea9d-158">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-158">Where the values originated if synced from another service.</span></span> <span data-ttu-id="1ea9d-159">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ea9d-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1ea9d-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="1ea9d-160">webUrl</span></span>|<span data-ttu-id="1ea9d-161">String</span><span class="sxs-lookup"><span data-stu-id="1ea9d-161">String</span></span>|<span data-ttu-id="1ea9d-162">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-162">Contains a link to an information source about the skill.</span></span> |

## <a name="response"></a><span data-ttu-id="1ea9d-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea9d-163">Response</span></span>

<span data-ttu-id="1ea9d-164">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [skillProficiency](../resources/skillproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-164">If successful, this method returns `201, Created` response code and a new [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ea9d-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1ea9d-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ea9d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea9d-166">Request</span></span>

<span data-ttu-id="1ea9d-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ea9d-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ea9d-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_skillproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/skills
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "allowedAudiences": "organization",
  "displayName": "API Design",
  "proficiency": "generalProfessional",
  "collaborationTags": [
    "ableToMentor"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="1ea9d-169">C#</span><span class="sxs-lookup"><span data-stu-id="1ea9d-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ea9d-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ea9d-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ea9d-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ea9d-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1ea9d-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea9d-172">Response</span></span>
<span data-ttu-id="1ea9d-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1ea9d-173">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


