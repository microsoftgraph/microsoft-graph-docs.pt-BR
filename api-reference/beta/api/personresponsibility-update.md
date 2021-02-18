---
title: Atualizar personResponsibility
description: Atualizar as propriedades de um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 62948aa9accfa79997e9a119f32d200cca507051
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292697"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="d3cb3-103">Atualizar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="d3cb3-103">Update personResponsibility</span></span>
<span data-ttu-id="d3cb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3cb3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3cb3-105">Atualizar as propriedades de [um objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="d3cb3-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3cb3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3cb3-106">Permissions</span></span>

<span data-ttu-id="d3cb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3cb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3cb3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3cb3-109">Permission type</span></span>                        | <span data-ttu-id="d3cb3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3cb3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d3cb3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3cb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3cb3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cb3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d3cb3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3cb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3cb3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cb3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d3cb3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3cb3-115">Application</span></span>                            | <span data-ttu-id="d3cb3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cb3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d3cb3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3cb3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3cb3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3cb3-118">Request headers</span></span>
|<span data-ttu-id="d3cb3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3cb3-119">Name</span></span>|<span data-ttu-id="d3cb3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3cb3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3cb3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3cb3-121">Authorization</span></span>|<span data-ttu-id="d3cb3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3cb3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3cb3-124">Content-Type</span></span>|<span data-ttu-id="d3cb3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3cb3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3cb3-127">Request body</span></span>
<span data-ttu-id="d3cb3-128">No corpo da solicitação, fornece uma representação JSON do [objeto personResponsibility.](../resources/personresponsibility.md)</span><span class="sxs-lookup"><span data-stu-id="d3cb3-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="d3cb3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [personResponsibility](../resources/personresponsibility.md).</span><span class="sxs-lookup"><span data-stu-id="d3cb3-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="d3cb3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3cb3-130">Property</span></span>|<span data-ttu-id="d3cb3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3cb3-131">Type</span></span>|<span data-ttu-id="d3cb3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3cb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3cb3-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d3cb3-133">allowedAudiences</span></span>|<span data-ttu-id="d3cb3-134">String</span><span class="sxs-lookup"><span data-stu-id="d3cb3-134">String</span></span>|<span data-ttu-id="d3cb3-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d3cb3-136">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d3cb3-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d3cb3-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d3cb3-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="d3cb3-138">collaborationTags</span></span>|<span data-ttu-id="d3cb3-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3cb3-139">String collection</span></span>|<span data-ttu-id="d3cb3-140">Contém marcas de cenário de experiência que um usuário associou ao interesse.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="d3cb3-141">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="d3cb3-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="d3cb3-142">description</span><span class="sxs-lookup"><span data-stu-id="d3cb3-142">description</span></span>|<span data-ttu-id="d3cb3-143">String</span><span class="sxs-lookup"><span data-stu-id="d3cb3-143">String</span></span>|<span data-ttu-id="d3cb3-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="d3cb3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d3cb3-145">displayName</span></span>|<span data-ttu-id="d3cb3-146">String</span><span class="sxs-lookup"><span data-stu-id="d3cb3-146">String</span></span>|<span data-ttu-id="d3cb3-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="d3cb3-148">inferência</span><span class="sxs-lookup"><span data-stu-id="d3cb3-148">inference</span></span>|[<span data-ttu-id="d3cb3-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d3cb3-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d3cb3-150">Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d3cb3-151">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d3cb3-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d3cb3-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="d3cb3-152">webUrl</span></span>|<span data-ttu-id="d3cb3-153">String</span><span class="sxs-lookup"><span data-stu-id="d3cb3-153">String</span></span>|<span data-ttu-id="d3cb3-154">Contém um link para uma página da Web ou recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="d3cb3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3cb3-155">Response</span></span>

<span data-ttu-id="d3cb3-156">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [personResponsibility](../resources/personresponsibility.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3cb3-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3cb3-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3cb3-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3cb3-158">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d3cb3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3cb3-159">Response</span></span>
<span data-ttu-id="d3cb3-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3cb3-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
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
  "source": null,
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


