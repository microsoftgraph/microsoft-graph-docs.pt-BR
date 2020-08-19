---
title: Criar PersonName
description: Use esta API para criar um novo PersonName no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ea4b8095d1af6e080e1e42162bbf1f8d56678446
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811616"
---
# <a name="create-personname"></a><span data-ttu-id="79cb5-103">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="79cb5-103">Create personName</span></span>

<span data-ttu-id="79cb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cb5-105">Use esta API para criar um novo objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79cb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79cb5-106">Permissions</span></span>

<span data-ttu-id="79cb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79cb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79cb5-109">Permission type</span></span>                        | <span data-ttu-id="79cb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79cb5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="79cb5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79cb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79cb5-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="79cb5-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79cb5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79cb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79cb5-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="79cb5-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79cb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79cb5-115">Application</span></span>                            | <span data-ttu-id="79cb5-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="79cb5-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79cb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79cb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="79cb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79cb5-118">Request headers</span></span>

| <span data-ttu-id="79cb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79cb5-119">Name</span></span>           |<span data-ttu-id="79cb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79cb5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="79cb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79cb5-121">Authorization</span></span>  | <span data-ttu-id="79cb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79cb5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="79cb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79cb5-124">Content-Type</span></span>   | <span data-ttu-id="79cb5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79cb5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79cb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79cb5-127">Request body</span></span>
<span data-ttu-id="79cb5-128">No corpo da solicitação, forneça uma representação JSON do objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="79cb5-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="79cb5-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="79cb5-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="79cb5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79cb5-130">Property</span></span>|<span data-ttu-id="79cb5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79cb5-131">Type</span></span>|<span data-ttu-id="79cb5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79cb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79cb5-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="79cb5-133">allowedAudiences</span></span>|<span data-ttu-id="79cb5-134">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-134">String</span></span>|<span data-ttu-id="79cb5-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="79cb5-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="79cb5-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="79cb5-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="79cb5-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="79cb5-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="79cb5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="79cb5-138">displayName</span></span>|<span data-ttu-id="79cb5-139">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-139">String</span></span>|<span data-ttu-id="79cb5-140">Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79cb5-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="79cb5-141">primeiro</span><span class="sxs-lookup"><span data-stu-id="79cb5-141">first</span></span>|<span data-ttu-id="79cb5-142">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-142">String</span></span>|<span data-ttu-id="79cb5-143">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-143">First name of the user.</span></span>|
|<span data-ttu-id="79cb5-144">id</span><span class="sxs-lookup"><span data-stu-id="79cb5-144">id</span></span>|<span data-ttu-id="79cb5-145">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-145">String</span></span>|<span data-ttu-id="79cb5-146">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="79cb5-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="79cb5-147">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="79cb5-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="79cb5-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="79cb5-148">inference</span></span>|[<span data-ttu-id="79cb5-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="79cb5-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="79cb5-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="79cb5-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="79cb5-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="79cb5-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="79cb5-152">initials</span><span class="sxs-lookup"><span data-stu-id="79cb5-152">initials</span></span>|<span data-ttu-id="79cb5-153">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-153">String</span></span>|<span data-ttu-id="79cb5-154">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-154">Initials of the user.</span></span>|
|<span data-ttu-id="79cb5-155">languageTag</span><span class="sxs-lookup"><span data-stu-id="79cb5-155">languageTag</span></span>|<span data-ttu-id="79cb5-156">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-156">String</span></span>|<span data-ttu-id="79cb5-157">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="79cb5-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="79cb5-158">durar</span><span class="sxs-lookup"><span data-stu-id="79cb5-158">last</span></span>|<span data-ttu-id="79cb5-159">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-159">String</span></span>|<span data-ttu-id="79cb5-160">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-160">Last name of the user.</span></span>|
|<span data-ttu-id="79cb5-161">Virgem</span><span class="sxs-lookup"><span data-stu-id="79cb5-161">maiden</span></span>|<span data-ttu-id="79cb5-162">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-162">String</span></span>|<span data-ttu-id="79cb5-163">Nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="79cb5-164">middleware</span><span class="sxs-lookup"><span data-stu-id="79cb5-164">middle</span></span>|<span data-ttu-id="79cb5-165">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-165">String</span></span>|<span data-ttu-id="79cb5-166">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-166">Middle name of the user.</span></span>|
|<span data-ttu-id="79cb5-167">apelido</span><span class="sxs-lookup"><span data-stu-id="79cb5-167">nickname</span></span>|<span data-ttu-id="79cb5-168">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-168">String</span></span>|<span data-ttu-id="79cb5-169">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="79cb5-169">Nickname of the user.</span></span>|
|<span data-ttu-id="79cb5-170">pronúncia</span><span class="sxs-lookup"><span data-stu-id="79cb5-170">pronunciation</span></span>|[<span data-ttu-id="79cb5-171">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="79cb5-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="79cb5-172">Orientações sobre como pronunciar o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="79cb5-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="79cb5-173">sufixo</span><span class="sxs-lookup"><span data-stu-id="79cb5-173">suffix</span></span>|<span data-ttu-id="79cb5-174">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-174">String</span></span>|<span data-ttu-id="79cb5-175">Designadores usados após o nome dos usuários (por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="79cb5-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="79cb5-176">title</span><span class="sxs-lookup"><span data-stu-id="79cb5-176">title</span></span>|<span data-ttu-id="79cb5-177">String</span><span class="sxs-lookup"><span data-stu-id="79cb5-177">String</span></span>|<span data-ttu-id="79cb5-178">Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="79cb5-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="79cb5-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="79cb5-179">Response</span></span>

<span data-ttu-id="79cb5-180">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79cb5-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79cb5-181">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79cb5-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79cb5-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79cb5-182">Request</span></span>

<span data-ttu-id="79cb5-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79cb5-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79cb5-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="79cb5-184">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null
}
```
# <a name="c"></a>[<span data-ttu-id="79cb5-185">C#</span><span class="sxs-lookup"><span data-stu-id="79cb5-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79cb5-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79cb5-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79cb5-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79cb5-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="79cb5-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="79cb5-188">Response</span></span>

<span data-ttu-id="79cb5-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79cb5-189">The following is an example of the response.</span></span>

> <span data-ttu-id="79cb5-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79cb5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
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
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": null,
  "suffix": null,
  "title": null,
  "pronunciation": null
}
```
