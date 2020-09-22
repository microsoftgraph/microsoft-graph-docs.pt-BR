---
title: Criar PersonName
description: Use esta API para criar um novo PersonName no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e410904881c588dd2e15deef008fda089210335f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034473"
---
# <a name="create-personname"></a><span data-ttu-id="4958d-103">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="4958d-103">Create personName</span></span>

<span data-ttu-id="4958d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4958d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4958d-105">Use esta API para criar um novo objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4958d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4958d-106">Permissions</span></span>

<span data-ttu-id="4958d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4958d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4958d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4958d-109">Permission type</span></span>                        | <span data-ttu-id="4958d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4958d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4958d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4958d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4958d-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4958d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4958d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4958d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4958d-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4958d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4958d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4958d-115">Application</span></span>                            | <span data-ttu-id="4958d-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4958d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4958d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4958d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="4958d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4958d-118">Request headers</span></span>

| <span data-ttu-id="4958d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4958d-119">Name</span></span>           |<span data-ttu-id="4958d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4958d-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4958d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4958d-121">Authorization</span></span>  | <span data-ttu-id="4958d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4958d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4958d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4958d-124">Content-Type</span></span>   | <span data-ttu-id="4958d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4958d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4958d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4958d-127">Request body</span></span>
<span data-ttu-id="4958d-128">No corpo da solicitação, forneça uma representação JSON do objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="4958d-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="4958d-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="4958d-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="4958d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4958d-130">Property</span></span>|<span data-ttu-id="4958d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4958d-131">Type</span></span>|<span data-ttu-id="4958d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4958d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4958d-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4958d-133">allowedAudiences</span></span>|<span data-ttu-id="4958d-134">String</span><span class="sxs-lookup"><span data-stu-id="4958d-134">String</span></span>|<span data-ttu-id="4958d-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="4958d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4958d-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4958d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4958d-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4958d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4958d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4958d-138">displayName</span></span>|<span data-ttu-id="4958d-139">String</span><span class="sxs-lookup"><span data-stu-id="4958d-139">String</span></span>|<span data-ttu-id="4958d-140">Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4958d-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="4958d-141">primeiro</span><span class="sxs-lookup"><span data-stu-id="4958d-141">first</span></span>|<span data-ttu-id="4958d-142">String</span><span class="sxs-lookup"><span data-stu-id="4958d-142">String</span></span>|<span data-ttu-id="4958d-143">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-143">First name of the user.</span></span>|
|<span data-ttu-id="4958d-144">id</span><span class="sxs-lookup"><span data-stu-id="4958d-144">id</span></span>|<span data-ttu-id="4958d-145">String</span><span class="sxs-lookup"><span data-stu-id="4958d-145">String</span></span>|<span data-ttu-id="4958d-146">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="4958d-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="4958d-147">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="4958d-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="4958d-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="4958d-148">inference</span></span>|[<span data-ttu-id="4958d-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4958d-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4958d-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="4958d-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4958d-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4958d-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4958d-152">initials</span><span class="sxs-lookup"><span data-stu-id="4958d-152">initials</span></span>|<span data-ttu-id="4958d-153">String</span><span class="sxs-lookup"><span data-stu-id="4958d-153">String</span></span>|<span data-ttu-id="4958d-154">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-154">Initials of the user.</span></span>|
|<span data-ttu-id="4958d-155">languageTag</span><span class="sxs-lookup"><span data-stu-id="4958d-155">languageTag</span></span>|<span data-ttu-id="4958d-156">String</span><span class="sxs-lookup"><span data-stu-id="4958d-156">String</span></span>|<span data-ttu-id="4958d-157">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="4958d-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="4958d-158">durar</span><span class="sxs-lookup"><span data-stu-id="4958d-158">last</span></span>|<span data-ttu-id="4958d-159">String</span><span class="sxs-lookup"><span data-stu-id="4958d-159">String</span></span>|<span data-ttu-id="4958d-160">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-160">Last name of the user.</span></span>|
|<span data-ttu-id="4958d-161">Virgem</span><span class="sxs-lookup"><span data-stu-id="4958d-161">maiden</span></span>|<span data-ttu-id="4958d-162">String</span><span class="sxs-lookup"><span data-stu-id="4958d-162">String</span></span>|<span data-ttu-id="4958d-163">Nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="4958d-164">middleware</span><span class="sxs-lookup"><span data-stu-id="4958d-164">middle</span></span>|<span data-ttu-id="4958d-165">String</span><span class="sxs-lookup"><span data-stu-id="4958d-165">String</span></span>|<span data-ttu-id="4958d-166">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-166">Middle name of the user.</span></span>|
|<span data-ttu-id="4958d-167">apelido</span><span class="sxs-lookup"><span data-stu-id="4958d-167">nickname</span></span>|<span data-ttu-id="4958d-168">String</span><span class="sxs-lookup"><span data-stu-id="4958d-168">String</span></span>|<span data-ttu-id="4958d-169">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="4958d-169">Nickname of the user.</span></span>|
|<span data-ttu-id="4958d-170">pronúncia</span><span class="sxs-lookup"><span data-stu-id="4958d-170">pronunciation</span></span>|[<span data-ttu-id="4958d-171">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="4958d-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="4958d-172">Orientações sobre como pronunciar o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="4958d-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="4958d-173">sufixo</span><span class="sxs-lookup"><span data-stu-id="4958d-173">suffix</span></span>|<span data-ttu-id="4958d-174">String</span><span class="sxs-lookup"><span data-stu-id="4958d-174">String</span></span>|<span data-ttu-id="4958d-175">Designadores usados após o nome dos usuários (por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="4958d-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="4958d-176">title</span><span class="sxs-lookup"><span data-stu-id="4958d-176">title</span></span>|<span data-ttu-id="4958d-177">String</span><span class="sxs-lookup"><span data-stu-id="4958d-177">String</span></span>|<span data-ttu-id="4958d-178">Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="4958d-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="4958d-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4958d-179">Response</span></span>

<span data-ttu-id="4958d-180">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4958d-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4958d-181">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4958d-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4958d-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4958d-182">Request</span></span>

<span data-ttu-id="4958d-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4958d-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4958d-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="4958d-184">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="4958d-185">C#</span><span class="sxs-lookup"><span data-stu-id="4958d-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4958d-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4958d-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4958d-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4958d-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4958d-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="4958d-188">Response</span></span>

<span data-ttu-id="4958d-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4958d-189">The following is an example of the response.</span></span>

> <span data-ttu-id="4958d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4958d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


