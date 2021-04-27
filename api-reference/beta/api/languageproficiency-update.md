---
title: Atualizar languageProficiency
description: Atualize as propriedades de um objeto languageProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5ab4d62d473fd07ddd202309b5345f0b8c07bd12
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049328"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="21385-103">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="21385-103">Update languageProficiency</span></span>

<span data-ttu-id="21385-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21385-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21385-105">Atualize as propriedades de [um objeto languageProficiency](../resources/languageproficiency.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="21385-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="21385-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="21385-106">Permissions</span></span>

<span data-ttu-id="21385-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21385-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21385-109">Permission type</span></span>                        | <span data-ttu-id="21385-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21385-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="21385-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21385-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="21385-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21385-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="21385-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21385-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21385-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21385-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="21385-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21385-115">Application</span></span>                            | <span data-ttu-id="21385-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21385-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="21385-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21385-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
PATCH /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21385-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21385-118">Request headers</span></span>

| <span data-ttu-id="21385-119">Nome</span><span class="sxs-lookup"><span data-stu-id="21385-119">Name</span></span>           |<span data-ttu-id="21385-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="21385-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="21385-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="21385-121">Authorization</span></span>  | <span data-ttu-id="21385-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21385-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="21385-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21385-124">Content-Type</span></span>   | <span data-ttu-id="21385-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21385-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21385-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21385-127">Request body</span></span>

<span data-ttu-id="21385-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="21385-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="21385-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="21385-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="21385-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="21385-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="21385-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21385-131">Property</span></span>|<span data-ttu-id="21385-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="21385-132">Type</span></span>|<span data-ttu-id="21385-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="21385-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21385-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="21385-134">allowedAudiences</span></span>|<span data-ttu-id="21385-135">String</span><span class="sxs-lookup"><span data-stu-id="21385-135">String</span></span>|<span data-ttu-id="21385-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="21385-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="21385-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="21385-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="21385-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21385-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21385-139">displayName</span><span class="sxs-lookup"><span data-stu-id="21385-139">displayName</span></span>|<span data-ttu-id="21385-140">String</span><span class="sxs-lookup"><span data-stu-id="21385-140">String</span></span>|<span data-ttu-id="21385-141">Contém o nome de formulário longo para o idioma.</span><span class="sxs-lookup"><span data-stu-id="21385-141">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="21385-142">inferência</span><span class="sxs-lookup"><span data-stu-id="21385-142">inference</span></span>|[<span data-ttu-id="21385-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="21385-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="21385-144">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="21385-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="21385-145">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="21385-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21385-146">leitura</span><span class="sxs-lookup"><span data-stu-id="21385-146">reading</span></span>|<span data-ttu-id="21385-147">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="21385-147">languageProficiencyLevel</span></span>|<span data-ttu-id="21385-148">Representa a compreensão de leitura dos usuários para o idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="21385-148">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="21385-149">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21385-149">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21385-150">source</span><span class="sxs-lookup"><span data-stu-id="21385-150">source</span></span>|[<span data-ttu-id="21385-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="21385-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="21385-152">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="21385-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="21385-153">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="21385-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21385-154">falado</span><span class="sxs-lookup"><span data-stu-id="21385-154">spoken</span></span>|<span data-ttu-id="21385-155">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="21385-155">languageProficiencyLevel</span></span>|<span data-ttu-id="21385-156">Representa a proficiência falada dos usuários para o idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="21385-156">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="21385-157">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21385-157">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21385-158">tag</span><span class="sxs-lookup"><span data-stu-id="21385-158">tag</span></span>|<span data-ttu-id="21385-159">String</span><span class="sxs-lookup"><span data-stu-id="21385-159">String</span></span>|<span data-ttu-id="21385-160">Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).</span><span class="sxs-lookup"><span data-stu-id="21385-160">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="21385-161">written</span><span class="sxs-lookup"><span data-stu-id="21385-161">written</span></span>|<span data-ttu-id="21385-162">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="21385-162">languageProficiencyLevel</span></span>|<span data-ttu-id="21385-163">Representa a proficiência escrita dos usuários para o idioma representado pelo objeto.</span><span class="sxs-lookup"><span data-stu-id="21385-163">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="21385-164">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21385-164">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="21385-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="21385-165">Response</span></span>

<span data-ttu-id="21385-166">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [languageProficiency](../resources/languageproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21385-166">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21385-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="21385-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21385-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21385-168">Request</span></span>

<span data-ttu-id="21385-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21385-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21385-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="21385-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="21385-171">C#</span><span class="sxs-lookup"><span data-stu-id="21385-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21385-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21385-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21385-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21385-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21385-174">Java</span><span class="sxs-lookup"><span data-stu-id="21385-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-languageproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="21385-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="21385-175">Response</span></span>

<span data-ttu-id="21385-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21385-176">The following is an example of the response.</span></span>

> <span data-ttu-id="21385-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21385-177">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
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
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```


