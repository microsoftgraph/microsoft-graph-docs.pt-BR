---
title: Criar responsabilidades
description: Crie um novo objeto de responsabilidade.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 086bc8af800c70a9282a04606f82818a135d65de
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440952"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="b3f75-103">Criar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="b3f75-103">Create personResponsibility</span></span>
<span data-ttu-id="b3f75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3f75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3f75-105">Criar um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="b3f75-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3f75-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3f75-106">Permissions</span></span>

<span data-ttu-id="b3f75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3f75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3f75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3f75-109">Permission type</span></span>                        | <span data-ttu-id="b3f75-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3f75-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b3f75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3f75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3f75-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3f75-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3f75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3f75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3f75-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3f75-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3f75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3f75-115">Application</span></span>                            | <span data-ttu-id="b3f75-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3f75-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b3f75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3f75-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="b3f75-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3f75-118">Request headers</span></span>
|<span data-ttu-id="b3f75-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b3f75-119">Name</span></span>|<span data-ttu-id="b3f75-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3f75-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3f75-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3f75-121">Authorization</span></span>|<span data-ttu-id="b3f75-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3f75-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b3f75-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3f75-124">Content-Type</span></span>|<span data-ttu-id="b3f75-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3f75-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3f75-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3f75-127">Request body</span></span>
<span data-ttu-id="b3f75-128">No corpo da solicitação, fornece uma representação JSON do [objeto personResponsibility.](../resources/personresponsibility.md)</span><span class="sxs-lookup"><span data-stu-id="b3f75-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="b3f75-129">A tabela a seguir mostra as propriedades que são possíveis de definir dentro de um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="b3f75-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="b3f75-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3f75-130">Property</span></span>|<span data-ttu-id="b3f75-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3f75-131">Type</span></span>|<span data-ttu-id="b3f75-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3f75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3f75-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b3f75-133">allowedAudiences</span></span>|<span data-ttu-id="b3f75-134">String</span><span class="sxs-lookup"><span data-stu-id="b3f75-134">String</span></span>|<span data-ttu-id="b3f75-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="b3f75-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b3f75-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b3f75-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b3f75-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b3f75-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b3f75-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="b3f75-138">collaborationTags</span></span>|<span data-ttu-id="b3f75-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3f75-139">String collection</span></span>|<span data-ttu-id="b3f75-140">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="b3f75-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="b3f75-141">Os valores permitidos na coleção são: `askMeAbout` `ableToMentor` , , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="b3f75-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="b3f75-142">descrição</span><span class="sxs-lookup"><span data-stu-id="b3f75-142">description</span></span>|<span data-ttu-id="b3f75-143">String</span><span class="sxs-lookup"><span data-stu-id="b3f75-143">String</span></span>|<span data-ttu-id="b3f75-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="b3f75-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="b3f75-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b3f75-145">displayName</span></span>|<span data-ttu-id="b3f75-146">String</span><span class="sxs-lookup"><span data-stu-id="b3f75-146">String</span></span>|<span data-ttu-id="b3f75-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="b3f75-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="b3f75-148">inferência</span><span class="sxs-lookup"><span data-stu-id="b3f75-148">inference</span></span>|[<span data-ttu-id="b3f75-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b3f75-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b3f75-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="b3f75-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b3f75-151">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b3f75-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b3f75-152">source</span><span class="sxs-lookup"><span data-stu-id="b3f75-152">source</span></span>|[<span data-ttu-id="b3f75-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="b3f75-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="b3f75-154">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f75-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="b3f75-155">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b3f75-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b3f75-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="b3f75-156">webUrl</span></span>|<span data-ttu-id="b3f75-157">String</span><span class="sxs-lookup"><span data-stu-id="b3f75-157">String</span></span>|<span data-ttu-id="b3f75-158">Contém um link para uma página da Web ou recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="b3f75-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="b3f75-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3f75-159">Response</span></span>

<span data-ttu-id="b3f75-160">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [personResponsibility](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3f75-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3f75-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b3f75-161">Examples</span></span>


# <a name="http"></a>[<span data-ttu-id="b3f75-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3f75-162">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b3f75-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3f75-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personresponsibility-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3f75-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3f75-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personresponsibility-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3f75-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3f75-165">Response</span></span>
<span data-ttu-id="b3f75-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b3f75-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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


