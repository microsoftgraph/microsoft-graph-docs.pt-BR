---
title: Criar responsabilidades
description: Crie um novo objeto de responsabilidades.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f46a7ba7e7e2d0a6b0d51d16059b78d286fe8e5a
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292340"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="5ba49-103">Criar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="5ba49-103">Create personResponsibility</span></span>
<span data-ttu-id="5ba49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ba49-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ba49-105">Crie um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5ba49-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ba49-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ba49-106">Permissions</span></span>

<span data-ttu-id="5ba49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ba49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ba49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ba49-109">Permission type</span></span>                        | <span data-ttu-id="5ba49-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ba49-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5ba49-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ba49-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ba49-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba49-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5ba49-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ba49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba49-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba49-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5ba49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ba49-115">Application</span></span>                            | <span data-ttu-id="5ba49-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba49-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5ba49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ba49-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="5ba49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ba49-118">Request headers</span></span>
|<span data-ttu-id="5ba49-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ba49-119">Name</span></span>|<span data-ttu-id="5ba49-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ba49-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ba49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ba49-121">Authorization</span></span>|<span data-ttu-id="5ba49-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ba49-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ba49-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ba49-124">Content-Type</span></span>|<span data-ttu-id="5ba49-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ba49-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ba49-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ba49-127">Request body</span></span>
<span data-ttu-id="5ba49-128">No corpo da solicitação, fornece uma representação JSON do [objeto personResponsibility.](../resources/personresponsibility.md)</span><span class="sxs-lookup"><span data-stu-id="5ba49-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="5ba49-129">A tabela a seguir mostra as propriedades que são possíveis definir em um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5ba49-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="5ba49-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ba49-130">Property</span></span>|<span data-ttu-id="5ba49-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ba49-131">Type</span></span>|<span data-ttu-id="5ba49-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ba49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ba49-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5ba49-133">allowedAudiences</span></span>|<span data-ttu-id="5ba49-134">String</span><span class="sxs-lookup"><span data-stu-id="5ba49-134">String</span></span>|<span data-ttu-id="5ba49-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="5ba49-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5ba49-136">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5ba49-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5ba49-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5ba49-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5ba49-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="5ba49-138">collaborationTags</span></span>|<span data-ttu-id="5ba49-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ba49-139">String collection</span></span>|<span data-ttu-id="5ba49-140">Contém marcas de cenário de experiência que um usuário associou ao interesse.</span><span class="sxs-lookup"><span data-stu-id="5ba49-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="5ba49-141">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="5ba49-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="5ba49-142">description</span><span class="sxs-lookup"><span data-stu-id="5ba49-142">description</span></span>|<span data-ttu-id="5ba49-143">String</span><span class="sxs-lookup"><span data-stu-id="5ba49-143">String</span></span>|<span data-ttu-id="5ba49-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="5ba49-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="5ba49-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5ba49-145">displayName</span></span>|<span data-ttu-id="5ba49-146">String</span><span class="sxs-lookup"><span data-stu-id="5ba49-146">String</span></span>|<span data-ttu-id="5ba49-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="5ba49-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="5ba49-148">inferência</span><span class="sxs-lookup"><span data-stu-id="5ba49-148">inference</span></span>|[<span data-ttu-id="5ba49-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5ba49-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5ba49-150">Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ba49-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5ba49-151">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5ba49-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5ba49-152">source</span><span class="sxs-lookup"><span data-stu-id="5ba49-152">source</span></span>|[<span data-ttu-id="5ba49-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5ba49-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5ba49-154">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="5ba49-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5ba49-155">Herdado de [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5ba49-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5ba49-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="5ba49-156">webUrl</span></span>|<span data-ttu-id="5ba49-157">String</span><span class="sxs-lookup"><span data-stu-id="5ba49-157">String</span></span>|<span data-ttu-id="5ba49-158">Contém um link para uma página da Web ou um recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="5ba49-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="5ba49-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ba49-159">Response</span></span>

<span data-ttu-id="5ba49-160">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto personResponsibility](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ba49-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ba49-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ba49-161">Examples</span></span>

<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5ba49-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ba49-162">Response</span></span>
<span data-ttu-id="5ba49-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ba49-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


