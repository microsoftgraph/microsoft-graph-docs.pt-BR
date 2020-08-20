---
title: Criar anotações
description: Criar um novo objeto Notes.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b7353c0a82b7a94fe61c92efc66df521e7fad4f3
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820191"
---
# <a name="create-personannotation"></a><span data-ttu-id="b604a-103">Criar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="b604a-103">Create personAnnotation</span></span>
<span data-ttu-id="b604a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b604a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b604a-105">Criar um novo objeto [personAnnotation](../resources/personannotation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b604a-105">Create a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b604a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b604a-106">Permissions</span></span>

<span data-ttu-id="b604a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b604a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b604a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b604a-109">Permission type</span></span>                        | <span data-ttu-id="b604a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b604a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b604a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b604a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b604a-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b604a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b604a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b604a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b604a-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b604a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b604a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b604a-115">Application</span></span>                            | <span data-ttu-id="b604a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b604a-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b604a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b604a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/notes
POST /users/{id | userPrincipalName}/profile/notes
```

## <a name="request-headers"></a><span data-ttu-id="b604a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b604a-118">Request headers</span></span>
|<span data-ttu-id="b604a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b604a-119">Name</span></span>|<span data-ttu-id="b604a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b604a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b604a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b604a-121">Authorization</span></span>|<span data-ttu-id="b604a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b604a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b604a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b604a-124">Content-Type</span></span>|<span data-ttu-id="b604a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b604a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b604a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b604a-127">Request body</span></span>
<span data-ttu-id="b604a-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAnnotation](../resources/personannotation.md) .</span><span class="sxs-lookup"><span data-stu-id="b604a-128">In the request body, supply a JSON representation of the [personAnnotation](../resources/personannotation.md) object.</span></span>

<span data-ttu-id="b604a-129">A tabela a seguir mostra as propriedades que são possíveis de definir em um novo objeto [personAnnotation](../resources/personannotation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b604a-129">The following table shows the properties that are possible to set within a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="b604a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b604a-130">Property</span></span>|<span data-ttu-id="b604a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b604a-131">Type</span></span>|<span data-ttu-id="b604a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b604a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b604a-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b604a-133">allowedAudiences</span></span>|<span data-ttu-id="b604a-134">String</span><span class="sxs-lookup"><span data-stu-id="b604a-134">String</span></span>|<span data-ttu-id="b604a-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="b604a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b604a-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b604a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b604a-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b604a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b604a-138">detalhada</span><span class="sxs-lookup"><span data-stu-id="b604a-138">detail</span></span>|[<span data-ttu-id="b604a-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="b604a-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="b604a-140">Contém os detalhes da anotação propriamente dita.</span><span class="sxs-lookup"><span data-stu-id="b604a-140">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="b604a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b604a-141">displayName</span></span>|<span data-ttu-id="b604a-142">String</span><span class="sxs-lookup"><span data-stu-id="b604a-142">String</span></span>|<span data-ttu-id="b604a-143">Contém um nome amigável para a anotação.</span><span class="sxs-lookup"><span data-stu-id="b604a-143">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="b604a-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="b604a-144">inference</span></span>|[<span data-ttu-id="b604a-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b604a-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b604a-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="b604a-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b604a-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b604a-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b604a-148">source</span><span class="sxs-lookup"><span data-stu-id="b604a-148">source</span></span>|[<span data-ttu-id="b604a-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="b604a-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="b604a-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="b604a-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="b604a-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b604a-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b604a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b604a-152">Response</span></span>

<span data-ttu-id="b604a-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personAnnotation](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b604a-153">If successful, this method returns a `201 Created` response code and a [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b604a-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b604a-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="b604a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b604a-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b604a-156">C#</span><span class="sxs-lookup"><span data-stu-id="b604a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personannotation-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b604a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b604a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personannotation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b604a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b604a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personannotation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b604a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b604a-159">Response</span></span>
<span data-ttu-id="b604a-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b604a-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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
