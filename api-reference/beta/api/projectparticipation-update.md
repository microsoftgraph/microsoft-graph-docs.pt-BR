---
title: Atualizar o tipo de recurso projectParticipation
description: Atualize as propriedades de um objeto projectParticipation no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5665c10cbaeb2968b5a17be3f7d30561ed9573d2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055194"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="65592-103">Atualizar projectparticipation</span><span class="sxs-lookup"><span data-stu-id="65592-103">Update projectparticipation</span></span>

<span data-ttu-id="65592-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65592-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65592-105">Atualize as propriedades de [um objeto projectParticipation](../resources/projectParticipation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="65592-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65592-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65592-106">Permissions</span></span>

<span data-ttu-id="65592-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65592-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65592-109">Permission type</span></span>                        | <span data-ttu-id="65592-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65592-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65592-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65592-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65592-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65592-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65592-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65592-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65592-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65592-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65592-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65592-115">Application</span></span>                            | <span data-ttu-id="65592-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65592-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="65592-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65592-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65592-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65592-118">Request headers</span></span>

| <span data-ttu-id="65592-119">Nome</span><span class="sxs-lookup"><span data-stu-id="65592-119">Name</span></span>           |<span data-ttu-id="65592-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="65592-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="65592-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="65592-121">Authorization</span></span>  | <span data-ttu-id="65592-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65592-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="65592-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65592-124">Content-Type</span></span>   | <span data-ttu-id="65592-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65592-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65592-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65592-127">Request body</span></span>

<span data-ttu-id="65592-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="65592-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="65592-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="65592-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="65592-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="65592-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="65592-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65592-131">Property</span></span>|<span data-ttu-id="65592-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="65592-132">Type</span></span>|<span data-ttu-id="65592-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="65592-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65592-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="65592-134">allowedAudiences</span></span>|<span data-ttu-id="65592-135">String</span><span class="sxs-lookup"><span data-stu-id="65592-135">String</span></span>|<span data-ttu-id="65592-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="65592-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="65592-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="65592-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="65592-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="65592-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="65592-139">categories</span><span class="sxs-lookup"><span data-stu-id="65592-139">categories</span></span>|<span data-ttu-id="65592-140">String collection</span><span class="sxs-lookup"><span data-stu-id="65592-140">String collection</span></span>|<span data-ttu-id="65592-141">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, plataforma de petróleo).</span><span class="sxs-lookup"><span data-stu-id="65592-141">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="65592-142">client</span><span class="sxs-lookup"><span data-stu-id="65592-142">client</span></span>|[<span data-ttu-id="65592-143">companyDetail</span><span class="sxs-lookup"><span data-stu-id="65592-143">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="65592-144">Contém informações detalhadas sobre o cliente para o que o projeto era.</span><span class="sxs-lookup"><span data-stu-id="65592-144">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="65592-145">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="65592-145">collaborationTags</span></span>|<span data-ttu-id="65592-146">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="65592-146">String collection</span></span>|<span data-ttu-id="65592-147">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="65592-147">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="65592-148">Os valores permitidos na coleção são: `askMeAbout` `ableToMentor` , , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="65592-148">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="65592-149">colleagues</span><span class="sxs-lookup"><span data-stu-id="65592-149">colleagues</span></span>|<span data-ttu-id="65592-150">[coleção relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="65592-150">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="65592-151">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="65592-151">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="65592-152">detail</span><span class="sxs-lookup"><span data-stu-id="65592-152">detail</span></span>|[<span data-ttu-id="65592-153">positionDetail</span><span class="sxs-lookup"><span data-stu-id="65592-153">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="65592-154">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="65592-154">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="65592-155">displayName</span><span class="sxs-lookup"><span data-stu-id="65592-155">displayName</span></span>|<span data-ttu-id="65592-156">String</span><span class="sxs-lookup"><span data-stu-id="65592-156">String</span></span>|<span data-ttu-id="65592-157">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="65592-157">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="65592-158">inferência</span><span class="sxs-lookup"><span data-stu-id="65592-158">inference</span></span>|[<span data-ttu-id="65592-159">inferenceData</span><span class="sxs-lookup"><span data-stu-id="65592-159">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="65592-160">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="65592-160">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="65592-161">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="65592-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="65592-162">patrocinadores</span><span class="sxs-lookup"><span data-stu-id="65592-162">sponsors</span></span>|<span data-ttu-id="65592-163">[coleção relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="65592-163">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="65592-164">A Pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="65592-164">The Person or people who sponsored the project.</span></span>    |

## <a name="response"></a><span data-ttu-id="65592-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="65592-165">Response</span></span>

<span data-ttu-id="65592-166">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto projectParticipation](../resources/projectparticipation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65592-166">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65592-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65592-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65592-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65592-168">Request</span></span>

<span data-ttu-id="65592-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65592-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65592-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="65592-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="65592-171">C#</span><span class="sxs-lookup"><span data-stu-id="65592-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65592-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65592-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65592-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65592-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65592-174">Java</span><span class="sxs-lookup"><span data-stu-id="65592-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-projectparticipation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65592-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="65592-175">Response</span></span>

<span data-ttu-id="65592-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65592-176">The following is an example of the response.</span></span>

> <span data-ttu-id="65592-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65592-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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


