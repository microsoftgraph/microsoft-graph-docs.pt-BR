---
title: Atualizar tipo de recurso projectParticipation
description: Atualiza as propriedades de um objeto projectParticipation no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c44ab0be22873ae37120d99ef86b70df586eb918
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010595"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="3da90-103">Atualizar projectparticipation</span><span class="sxs-lookup"><span data-stu-id="3da90-103">Update projectparticipation</span></span>

<span data-ttu-id="3da90-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3da90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da90-105">Atualiza as propriedades de um objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3da90-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3da90-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3da90-106">Permissions</span></span>

<span data-ttu-id="3da90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3da90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3da90-109">Permission type</span></span>                        | <span data-ttu-id="3da90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3da90-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3da90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3da90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3da90-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3da90-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3da90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3da90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3da90-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3da90-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3da90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3da90-115">Application</span></span>                            | <span data-ttu-id="3da90-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da90-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3da90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3da90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3da90-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3da90-118">Request headers</span></span>

| <span data-ttu-id="3da90-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3da90-119">Name</span></span>           |<span data-ttu-id="3da90-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da90-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3da90-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3da90-121">Authorization</span></span>  | <span data-ttu-id="3da90-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3da90-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3da90-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3da90-124">Content-Type</span></span>   | <span data-ttu-id="3da90-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3da90-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3da90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3da90-127">Request body</span></span>

<span data-ttu-id="3da90-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="3da90-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3da90-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="3da90-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3da90-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3da90-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="3da90-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3da90-131">Property</span></span>|<span data-ttu-id="3da90-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3da90-132">Type</span></span>|<span data-ttu-id="3da90-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da90-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da90-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="3da90-134">allowedAudiences</span></span>|<span data-ttu-id="3da90-135">String</span><span class="sxs-lookup"><span data-stu-id="3da90-135">String</span></span>|<span data-ttu-id="3da90-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="3da90-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="3da90-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3da90-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="3da90-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3da90-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3da90-139">Categorias</span><span class="sxs-lookup"><span data-stu-id="3da90-139">categories</span></span>|<span data-ttu-id="3da90-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3da90-140">String collection</span></span>|<span data-ttu-id="3da90-141">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo).</span><span class="sxs-lookup"><span data-stu-id="3da90-141">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="3da90-142">clientes</span><span class="sxs-lookup"><span data-stu-id="3da90-142">client</span></span>|[<span data-ttu-id="3da90-143">companyDetail</span><span class="sxs-lookup"><span data-stu-id="3da90-143">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="3da90-144">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="3da90-144">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="3da90-145">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="3da90-145">collaborationTags</span></span>|<span data-ttu-id="3da90-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3da90-146">String collection</span></span>|<span data-ttu-id="3da90-147">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="3da90-147">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="3da90-148">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="3da90-148">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="3da90-149">conhecidos</span><span class="sxs-lookup"><span data-stu-id="3da90-149">colleagues</span></span>|<span data-ttu-id="3da90-150">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3da90-150">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="3da90-151">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="3da90-151">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="3da90-152">detalhada</span><span class="sxs-lookup"><span data-stu-id="3da90-152">detail</span></span>|[<span data-ttu-id="3da90-153">positionDetail</span><span class="sxs-lookup"><span data-stu-id="3da90-153">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="3da90-154">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="3da90-154">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="3da90-155">displayName</span><span class="sxs-lookup"><span data-stu-id="3da90-155">displayName</span></span>|<span data-ttu-id="3da90-156">String</span><span class="sxs-lookup"><span data-stu-id="3da90-156">String</span></span>|<span data-ttu-id="3da90-157">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="3da90-157">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="3da90-158">fracassa</span><span class="sxs-lookup"><span data-stu-id="3da90-158">inference</span></span>|[<span data-ttu-id="3da90-159">inferenceData</span><span class="sxs-lookup"><span data-stu-id="3da90-159">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="3da90-160">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="3da90-160">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="3da90-161">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3da90-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3da90-162">responsáveis</span><span class="sxs-lookup"><span data-stu-id="3da90-162">sponsors</span></span>|<span data-ttu-id="3da90-163">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3da90-163">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="3da90-164">A pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="3da90-164">The Person or people who sponsored the project.</span></span>    |

## <a name="response"></a><span data-ttu-id="3da90-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da90-165">Response</span></span>

<span data-ttu-id="3da90-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [projectParticipation](../resources/projectparticipation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3da90-166">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3da90-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3da90-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3da90-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3da90-168">Request</span></span>

<span data-ttu-id="3da90-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3da90-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3da90-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="3da90-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "allowedAudiences": "organization",
  "client": {
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="3da90-171">C#</span><span class="sxs-lookup"><span data-stu-id="3da90-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3da90-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3da90-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3da90-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3da90-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3da90-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da90-174">Response</span></span>

<span data-ttu-id="3da90-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3da90-175">The following is an example of the response.</span></span>

> <span data-ttu-id="3da90-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3da90-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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


