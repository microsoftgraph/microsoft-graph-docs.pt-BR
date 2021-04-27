---
title: Atualizar personName
description: Atualize as propriedades de um objeto personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0959c7eec1b1e52ff3a9295ad7e5af07b416a3bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051099"
---
# <a name="update-personname"></a><span data-ttu-id="33b89-103">Atualizar nome de pessoa</span><span class="sxs-lookup"><span data-stu-id="33b89-103">Update personname</span></span>

<span data-ttu-id="33b89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33b89-105">Atualize as propriedades de [um objeto personName](../resources/personname.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="33b89-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33b89-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33b89-106">Permissions</span></span>

<span data-ttu-id="33b89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33b89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b89-109">Permission type</span></span>                        | <span data-ttu-id="33b89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33b89-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="33b89-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b89-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33b89-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b89-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="33b89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b89-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b89-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="33b89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b89-115">Application</span></span>                            | <span data-ttu-id="33b89-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b89-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="33b89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b89-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="33b89-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b89-118">Request headers</span></span>

| <span data-ttu-id="33b89-119">Nome</span><span class="sxs-lookup"><span data-stu-id="33b89-119">Name</span></span>           |<span data-ttu-id="33b89-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b89-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="33b89-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b89-121">Authorization</span></span>  | <span data-ttu-id="33b89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b89-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="33b89-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33b89-124">Content-Type</span></span>   | <span data-ttu-id="33b89-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b89-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33b89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b89-127">Request body</span></span>

<span data-ttu-id="33b89-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="33b89-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="33b89-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="33b89-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="33b89-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="33b89-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="33b89-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar dentro de um [objeto personName](../resources/personname.md) existente no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="33b89-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="33b89-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33b89-132">Property</span></span>|<span data-ttu-id="33b89-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="33b89-133">Type</span></span>|<span data-ttu-id="33b89-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b89-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b89-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="33b89-135">allowedAudiences</span></span>|<span data-ttu-id="33b89-136">String</span><span class="sxs-lookup"><span data-stu-id="33b89-136">String</span></span>|<span data-ttu-id="33b89-137">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="33b89-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="33b89-138">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="33b89-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="33b89-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="33b89-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="33b89-140">displayName</span><span class="sxs-lookup"><span data-stu-id="33b89-140">displayName</span></span>|<span data-ttu-id="33b89-141">String</span><span class="sxs-lookup"><span data-stu-id="33b89-141">String</span></span>|<span data-ttu-id="33b89-142">Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33b89-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="33b89-143">first</span><span class="sxs-lookup"><span data-stu-id="33b89-143">first</span></span>|<span data-ttu-id="33b89-144">String</span><span class="sxs-lookup"><span data-stu-id="33b89-144">String</span></span>|<span data-ttu-id="33b89-145">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-145">First name of the user.</span></span>|
|<span data-ttu-id="33b89-146">inferência</span><span class="sxs-lookup"><span data-stu-id="33b89-146">inference</span></span>|[<span data-ttu-id="33b89-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="33b89-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="33b89-148">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="33b89-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="33b89-149">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="33b89-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="33b89-150">initials</span><span class="sxs-lookup"><span data-stu-id="33b89-150">initials</span></span>|<span data-ttu-id="33b89-151">String</span><span class="sxs-lookup"><span data-stu-id="33b89-151">String</span></span>|<span data-ttu-id="33b89-152">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-152">Initials of the user.</span></span>|
|<span data-ttu-id="33b89-153">languageTag</span><span class="sxs-lookup"><span data-stu-id="33b89-153">languageTag</span></span>|<span data-ttu-id="33b89-154">String</span><span class="sxs-lookup"><span data-stu-id="33b89-154">String</span></span>|<span data-ttu-id="33b89-155">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="33b89-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="33b89-156">last</span><span class="sxs-lookup"><span data-stu-id="33b89-156">last</span></span>|<span data-ttu-id="33b89-157">String</span><span class="sxs-lookup"><span data-stu-id="33b89-157">String</span></span>|<span data-ttu-id="33b89-158">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-158">Last name of the user.</span></span>|
|<span data-ttu-id="33b89-159">maiden</span><span class="sxs-lookup"><span data-stu-id="33b89-159">maiden</span></span>|<span data-ttu-id="33b89-160">String</span><span class="sxs-lookup"><span data-stu-id="33b89-160">String</span></span>|<span data-ttu-id="33b89-161">Nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="33b89-162">middle</span><span class="sxs-lookup"><span data-stu-id="33b89-162">middle</span></span>|<span data-ttu-id="33b89-163">String</span><span class="sxs-lookup"><span data-stu-id="33b89-163">String</span></span>|<span data-ttu-id="33b89-164">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-164">Middle name of the user.</span></span>|
|<span data-ttu-id="33b89-165">nickname</span><span class="sxs-lookup"><span data-stu-id="33b89-165">nickname</span></span>|<span data-ttu-id="33b89-166">String</span><span class="sxs-lookup"><span data-stu-id="33b89-166">String</span></span>|<span data-ttu-id="33b89-167">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b89-167">Nickname of the user.</span></span>|
|<span data-ttu-id="33b89-168">pronúncia</span><span class="sxs-lookup"><span data-stu-id="33b89-168">pronunciation</span></span>|[<span data-ttu-id="33b89-169">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="33b89-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="33b89-170">Diretrizes sobre como pronunciar o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="33b89-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="33b89-171">sufixo</span><span class="sxs-lookup"><span data-stu-id="33b89-171">suffix</span></span>|<span data-ttu-id="33b89-172">String</span><span class="sxs-lookup"><span data-stu-id="33b89-172">String</span></span>|<span data-ttu-id="33b89-173">Designadores usados após o nome dos usuários (por exemplo: PhD.)</span><span class="sxs-lookup"><span data-stu-id="33b89-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="33b89-174">title</span><span class="sxs-lookup"><span data-stu-id="33b89-174">title</span></span>|<span data-ttu-id="33b89-175">String</span><span class="sxs-lookup"><span data-stu-id="33b89-175">String</span></span>|<span data-ttu-id="33b89-176">Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Mrs.)</span><span class="sxs-lookup"><span data-stu-id="33b89-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="33b89-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b89-177">Response</span></span>

<span data-ttu-id="33b89-178">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto personName](../resources/personname.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b89-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33b89-179">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33b89-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33b89-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b89-180">Request</span></span>

<span data-ttu-id="33b89-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b89-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33b89-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="33b89-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "nickname": "Kesha"
}

```
# <a name="c"></a>[<span data-ttu-id="33b89-183">C#</span><span class="sxs-lookup"><span data-stu-id="33b89-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33b89-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33b89-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33b89-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33b89-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33b89-186">Java</span><span class="sxs-lookup"><span data-stu-id="33b89-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="33b89-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b89-187">Response</span></span>

<span data-ttu-id="33b89-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33b89-188">The following is an example of the response.</span></span>

> <span data-ttu-id="33b89-189">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33b89-189">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
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
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "displayName": "In-no ken-te ",
    "first": "In-no ken-te Pop-ov",
    "maiden": null,
    "middle": null,
    "last": "Pop-ov"
  }
}
```


