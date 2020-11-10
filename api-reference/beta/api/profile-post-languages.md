---
title: Criar languageProficiency
description: Use esta API para criar um novo languageProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 38e46c90841e48358cef9fc4f7f486c2ea5da2e7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979583"
---
# <a name="create-languageproficiency"></a><span data-ttu-id="68150-103">Criar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="68150-103">Create languageProficiency</span></span>

<span data-ttu-id="68150-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68150-105">Use esta API para criar um novo objeto [languageProficiency](../resources/languageproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="68150-105">Use this API to create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68150-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68150-106">Permissions</span></span>

<span data-ttu-id="68150-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68150-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68150-109">Permission type</span></span>                        | <span data-ttu-id="68150-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68150-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68150-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68150-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68150-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68150-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="68150-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68150-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68150-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68150-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="68150-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68150-115">Application</span></span>                            | <span data-ttu-id="68150-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68150-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="68150-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68150-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/languages
POST /users/{id | userPrincipalName}/profile/languages
```

## <a name="request-headers"></a><span data-ttu-id="68150-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68150-118">Request headers</span></span>

| <span data-ttu-id="68150-119">Nome</span><span class="sxs-lookup"><span data-stu-id="68150-119">Name</span></span>           | <span data-ttu-id="68150-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68150-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="68150-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68150-121">Authorization</span></span>  | <span data-ttu-id="68150-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68150-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="68150-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68150-124">Content-Type</span></span>   | <span data-ttu-id="68150-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68150-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68150-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68150-127">Request body</span></span>

<span data-ttu-id="68150-128">No corpo da solicitação, forneça uma representação JSON do objeto [languageProficiency](../resources/languageproficiency.md) .</span><span class="sxs-lookup"><span data-stu-id="68150-128">In the request body, supply a JSON representation of [languageProficiency](../resources/languageproficiency.md) object.</span></span>

<span data-ttu-id="68150-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [languageProficiency](../resources/languageproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="68150-129">The following table shows the properties that are possible to set when you create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="68150-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68150-130">Property</span></span>|<span data-ttu-id="68150-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="68150-131">Type</span></span>|<span data-ttu-id="68150-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="68150-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68150-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="68150-133">allowedAudiences</span></span>|<span data-ttu-id="68150-134">String</span><span class="sxs-lookup"><span data-stu-id="68150-134">String</span></span>|<span data-ttu-id="68150-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="68150-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="68150-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="68150-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="68150-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68150-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="68150-138">displayName</span><span class="sxs-lookup"><span data-stu-id="68150-138">displayName</span></span>|<span data-ttu-id="68150-139">String</span><span class="sxs-lookup"><span data-stu-id="68150-139">String</span></span>|<span data-ttu-id="68150-140">Contém o nome de formato longo para o idioma.</span><span class="sxs-lookup"><span data-stu-id="68150-140">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="68150-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="68150-141">inference</span></span>|[<span data-ttu-id="68150-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="68150-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="68150-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="68150-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="68150-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="68150-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="68150-145">Converte</span><span class="sxs-lookup"><span data-stu-id="68150-145">reading</span></span>|<span data-ttu-id="68150-146">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="68150-146">languageProficiencyLevel</span></span>|<span data-ttu-id="68150-147">Representa os usuários que estão lendo a compreensão do idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="68150-147">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="68150-148">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68150-148">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="68150-149">source</span><span class="sxs-lookup"><span data-stu-id="68150-149">source</span></span>|[<span data-ttu-id="68150-150">personDataSource</span><span class="sxs-lookup"><span data-stu-id="68150-150">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="68150-151">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="68150-151">Where the values originated if synced from another service.</span></span> <span data-ttu-id="68150-152">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="68150-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="68150-153">idioma</span><span class="sxs-lookup"><span data-stu-id="68150-153">spoken</span></span>|<span data-ttu-id="68150-154">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="68150-154">languageProficiencyLevel</span></span>|<span data-ttu-id="68150-155">Representa a proficiência dos usuários falada sobre o idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="68150-155">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="68150-156">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68150-156">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="68150-157">tag</span><span class="sxs-lookup"><span data-stu-id="68150-157">tag</span></span>|<span data-ttu-id="68150-158">String</span><span class="sxs-lookup"><span data-stu-id="68150-158">String</span></span>|<span data-ttu-id="68150-159">Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).</span><span class="sxs-lookup"><span data-stu-id="68150-159">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="68150-160">pré-gravados</span><span class="sxs-lookup"><span data-stu-id="68150-160">written</span></span>|<span data-ttu-id="68150-161">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="68150-161">languageProficiencyLevel</span></span>|<span data-ttu-id="68150-162">Representa a proficiência dos usuários gravados para o idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="68150-162">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="68150-163">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68150-163">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="68150-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="68150-164">Response</span></span>

<span data-ttu-id="68150-165">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [languageProficiency](../resources/languageproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68150-165">If successful, this method returns `201, Created` response code and a new [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68150-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68150-166">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68150-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68150-167">Request</span></span>

<span data-ttu-id="68150-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68150-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68150-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="68150-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_languageproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/languages
Content-type: application/json

{
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```
# <a name="c"></a>[<span data-ttu-id="68150-170">C#</span><span class="sxs-lookup"><span data-stu-id="68150-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-languageproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68150-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68150-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-languageproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68150-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68150-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-languageproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68150-173">Java</span><span class="sxs-lookup"><span data-stu-id="68150-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-languageproficiency-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68150-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="68150-174">Response</span></span>

<span data-ttu-id="68150-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68150-175">The following is an example of the response.</span></span>

> <span data-ttu-id="68150-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68150-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
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
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```


