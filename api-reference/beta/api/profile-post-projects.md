---
title: Criar projectParticipation
description: Use esta API para criar um novo projectParticipation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b3e2cae6b14f3e7f8ea336bb3000bfa8e4894ac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034396"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="3043f-103">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3043f-103">Create projectParticipation</span></span>

<span data-ttu-id="3043f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3043f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3043f-105">Use esta API para criar um novo objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3043f-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3043f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3043f-106">Permissions</span></span>

<span data-ttu-id="3043f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3043f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3043f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3043f-109">Permission type</span></span>                        | <span data-ttu-id="3043f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3043f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3043f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3043f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3043f-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3043f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3043f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3043f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3043f-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3043f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3043f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3043f-115">Application</span></span>                            | <span data-ttu-id="3043f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3043f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3043f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3043f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
POST /users/{id | userPrincipalName}/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="3043f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3043f-118">Request headers</span></span>

| <span data-ttu-id="3043f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3043f-119">Name</span></span>           |<span data-ttu-id="3043f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3043f-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="3043f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3043f-121">Authorization</span></span>  | <span data-ttu-id="3043f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3043f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3043f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3043f-124">Content-Type</span></span>   | <span data-ttu-id="3043f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3043f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3043f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3043f-127">Request body</span></span>

<span data-ttu-id="3043f-128">No corpo da solicitação, forneça uma representação JSON do objeto [projectParticipation](../resources/projectparticipation.md) .</span><span class="sxs-lookup"><span data-stu-id="3043f-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

<span data-ttu-id="3043f-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3043f-129">The following table shows the properties that are possible to set when you create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="3043f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3043f-130">Property</span></span>|<span data-ttu-id="3043f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3043f-131">Type</span></span>|<span data-ttu-id="3043f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3043f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3043f-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="3043f-133">allowedAudiences</span></span>|<span data-ttu-id="3043f-134">String</span><span class="sxs-lookup"><span data-stu-id="3043f-134">String</span></span>|<span data-ttu-id="3043f-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="3043f-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="3043f-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3043f-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="3043f-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3043f-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3043f-138">categories</span><span class="sxs-lookup"><span data-stu-id="3043f-138">categories</span></span>|<span data-ttu-id="3043f-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3043f-139">String collection</span></span>|<span data-ttu-id="3043f-140">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo).</span><span class="sxs-lookup"><span data-stu-id="3043f-140">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="3043f-141">clientes</span><span class="sxs-lookup"><span data-stu-id="3043f-141">client</span></span>|[<span data-ttu-id="3043f-142">companyDetail</span><span class="sxs-lookup"><span data-stu-id="3043f-142">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="3043f-143">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="3043f-143">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="3043f-144">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="3043f-144">collaborationTags</span></span>|<span data-ttu-id="3043f-145">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3043f-145">String collection</span></span>|<span data-ttu-id="3043f-146">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="3043f-146">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="3043f-147">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="3043f-147">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="3043f-148">conhecidos</span><span class="sxs-lookup"><span data-stu-id="3043f-148">colleagues</span></span>|<span data-ttu-id="3043f-149">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3043f-149">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="3043f-150">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="3043f-150">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="3043f-151">detalhada</span><span class="sxs-lookup"><span data-stu-id="3043f-151">detail</span></span>|[<span data-ttu-id="3043f-152">positionDetail</span><span class="sxs-lookup"><span data-stu-id="3043f-152">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="3043f-153">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="3043f-153">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="3043f-154">displayName</span><span class="sxs-lookup"><span data-stu-id="3043f-154">displayName</span></span>|<span data-ttu-id="3043f-155">String</span><span class="sxs-lookup"><span data-stu-id="3043f-155">String</span></span>|<span data-ttu-id="3043f-156">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="3043f-156">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="3043f-157">fracassa</span><span class="sxs-lookup"><span data-stu-id="3043f-157">inference</span></span>|[<span data-ttu-id="3043f-158">inferenceData</span><span class="sxs-lookup"><span data-stu-id="3043f-158">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="3043f-159">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="3043f-159">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="3043f-160">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3043f-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3043f-161">source</span><span class="sxs-lookup"><span data-stu-id="3043f-161">source</span></span>|[<span data-ttu-id="3043f-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="3043f-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="3043f-163">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="3043f-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="3043f-164">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3043f-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3043f-165">responsáveis</span><span class="sxs-lookup"><span data-stu-id="3043f-165">sponsors</span></span>|<span data-ttu-id="3043f-166">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3043f-166">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="3043f-167">A pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="3043f-167">The Person or people who sponsored the project.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="3043f-168">Relações</span><span class="sxs-lookup"><span data-stu-id="3043f-168">Relationships</span></span>

## <a name="response"></a><span data-ttu-id="3043f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="3043f-169">Response</span></span>

<span data-ttu-id="3043f-170">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [projectParticipation](../resources/projectparticipation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3043f-170">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3043f-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3043f-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3043f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3043f-172">Request</span></span>

<span data-ttu-id="3043f-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3043f-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3043f-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="3043f-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "department": "Consulting",
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  }
}
```
# <a name="c"></a>[<span data-ttu-id="3043f-175">C#</span><span class="sxs-lookup"><span data-stu-id="3043f-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3043f-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3043f-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3043f-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3043f-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3043f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="3043f-178">Response</span></span>

<span data-ttu-id="3043f-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3043f-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3043f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3043f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "pronunciation": null,
    "department": "Corporate Marketing",
    "officeLocation": null,
    "address": null,
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": null,
      "address": null,
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "endMonthYear": "datetime-value",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "startMonthYear": "datetime-value",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  },
  "colleagues": null,
  "sponsors": null
}
```


