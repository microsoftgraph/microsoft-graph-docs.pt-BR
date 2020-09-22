---
title: Criar anotações
description: Criar um novo objeto Notes.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 139de864b9ddec90336e56e122da5f6bf6922952
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034383"
---
# <a name="create-personannotation"></a><span data-ttu-id="92ff7-103">Criar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="92ff7-103">Create personAnnotation</span></span>
<span data-ttu-id="92ff7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ff7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92ff7-105">Criar um novo objeto [personAnnotation](../resources/personannotation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="92ff7-105">Create a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92ff7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92ff7-106">Permissions</span></span>

<span data-ttu-id="92ff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92ff7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92ff7-109">Permission type</span></span>                        | <span data-ttu-id="92ff7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92ff7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="92ff7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92ff7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92ff7-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92ff7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="92ff7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92ff7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ff7-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92ff7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="92ff7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92ff7-115">Application</span></span>                            | <span data-ttu-id="92ff7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ff7-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="92ff7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92ff7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/notes
POST /users/{id | userPrincipalName}/profile/notes
```

## <a name="request-headers"></a><span data-ttu-id="92ff7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92ff7-118">Request headers</span></span>
|<span data-ttu-id="92ff7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="92ff7-119">Name</span></span>|<span data-ttu-id="92ff7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ff7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="92ff7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="92ff7-121">Authorization</span></span>|<span data-ttu-id="92ff7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ff7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="92ff7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92ff7-124">Content-Type</span></span>|<span data-ttu-id="92ff7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ff7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ff7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92ff7-127">Request body</span></span>
<span data-ttu-id="92ff7-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAnnotation](../resources/personannotation.md) .</span><span class="sxs-lookup"><span data-stu-id="92ff7-128">In the request body, supply a JSON representation of the [personAnnotation](../resources/personannotation.md) object.</span></span>

<span data-ttu-id="92ff7-129">A tabela a seguir mostra as propriedades que são possíveis de definir em um novo objeto [personAnnotation](../resources/personannotation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="92ff7-129">The following table shows the properties that are possible to set within a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="92ff7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92ff7-130">Property</span></span>|<span data-ttu-id="92ff7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ff7-131">Type</span></span>|<span data-ttu-id="92ff7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ff7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ff7-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="92ff7-133">allowedAudiences</span></span>|<span data-ttu-id="92ff7-134">String</span><span class="sxs-lookup"><span data-stu-id="92ff7-134">String</span></span>|<span data-ttu-id="92ff7-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="92ff7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="92ff7-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="92ff7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="92ff7-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="92ff7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="92ff7-138">detalhada</span><span class="sxs-lookup"><span data-stu-id="92ff7-138">detail</span></span>|[<span data-ttu-id="92ff7-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="92ff7-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="92ff7-140">Contém os detalhes da anotação propriamente dita.</span><span class="sxs-lookup"><span data-stu-id="92ff7-140">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="92ff7-141">displayName</span><span class="sxs-lookup"><span data-stu-id="92ff7-141">displayName</span></span>|<span data-ttu-id="92ff7-142">String</span><span class="sxs-lookup"><span data-stu-id="92ff7-142">String</span></span>|<span data-ttu-id="92ff7-143">Contém um nome amigável para a anotação.</span><span class="sxs-lookup"><span data-stu-id="92ff7-143">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="92ff7-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="92ff7-144">inference</span></span>|[<span data-ttu-id="92ff7-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="92ff7-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="92ff7-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="92ff7-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="92ff7-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="92ff7-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="92ff7-148">source</span><span class="sxs-lookup"><span data-stu-id="92ff7-148">source</span></span>|[<span data-ttu-id="92ff7-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="92ff7-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="92ff7-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="92ff7-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="92ff7-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="92ff7-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="92ff7-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ff7-152">Response</span></span>

<span data-ttu-id="92ff7-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personAnnotation](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92ff7-153">If successful, this method returns a `201 Created` response code and a [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92ff7-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92ff7-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="92ff7-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="92ff7-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personannotation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/notes
Content-Type: application/json
Content-length: 413

{
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```
# <a name="c"></a>[<span data-ttu-id="92ff7-156">C#</span><span class="sxs-lookup"><span data-stu-id="92ff7-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personannotation-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92ff7-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92ff7-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personannotation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92ff7-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92ff7-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personannotation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92ff7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ff7-159">Response</span></span>
<span data-ttu-id="92ff7-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92ff7-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnnotation"
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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```


