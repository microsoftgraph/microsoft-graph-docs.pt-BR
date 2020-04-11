---
title: Atualizar PersonName
description: Atualiza as propriedades de um objeto PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 26989c4eb5b7af987ab9a50555d3abdf07e3a16a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228688"
---
# <a name="update-personname"></a><span data-ttu-id="f95b1-103">Atualizar PersonName</span><span class="sxs-lookup"><span data-stu-id="f95b1-103">Update personname</span></span>

<span data-ttu-id="f95b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f95b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f95b1-105">Atualiza as propriedades de um objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f95b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f95b1-106">Permissions</span></span>

<span data-ttu-id="f95b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f95b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f95b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f95b1-109">Permission type</span></span>                        | <span data-ttu-id="f95b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f95b1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f95b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f95b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f95b1-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f95b1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f95b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f95b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f95b1-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f95b1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f95b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f95b1-115">Application</span></span>                            | <span data-ttu-id="f95b1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95b1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f95b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f95b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f95b1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b1-118">Request headers</span></span>

| <span data-ttu-id="f95b1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f95b1-119">Name</span></span>           |<span data-ttu-id="f95b1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95b1-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f95b1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f95b1-121">Authorization</span></span>  | <span data-ttu-id="f95b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f95b1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f95b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f95b1-124">Content-Type</span></span>   | <span data-ttu-id="f95b1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f95b1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f95b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b1-127">Request body</span></span>

<span data-ttu-id="f95b1-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f95b1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f95b1-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f95b1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f95b1-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f95b1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f95b1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f95b1-131">Property</span></span>     | <span data-ttu-id="f95b1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f95b1-132">Type</span></span>                                            | <span data-ttu-id="f95b1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95b1-133">Description</span></span>                                                                             |
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="f95b1-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f95b1-134">displayName</span></span>   |<span data-ttu-id="f95b1-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f95b1-135">String</span></span>                                           | <span data-ttu-id="f95b1-136">Fornece um processamento ordenado de nome e sobrenome.</span><span class="sxs-lookup"><span data-stu-id="f95b1-136">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="f95b1-137">primeiro</span><span class="sxs-lookup"><span data-stu-id="f95b1-137">first</span></span>         |<span data-ttu-id="f95b1-138">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-138">String</span></span>                                           | <span data-ttu-id="f95b1-139">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-139">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="f95b1-140">initials</span><span class="sxs-lookup"><span data-stu-id="f95b1-140">initials</span></span>      |<span data-ttu-id="f95b1-141">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-141">String</span></span>                                           | <span data-ttu-id="f95b1-142">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-142">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="f95b1-143">languageTag</span><span class="sxs-lookup"><span data-stu-id="f95b1-143">languageTag</span></span>   |<span data-ttu-id="f95b1-144">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-144">String</span></span>                                           | <span data-ttu-id="f95b1-145">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="f95b1-145">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="f95b1-146">durar</span><span class="sxs-lookup"><span data-stu-id="f95b1-146">last</span></span>          |<span data-ttu-id="f95b1-147">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-147">String</span></span>                                           | <span data-ttu-id="f95b1-148">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-148">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="f95b1-149">Virgem</span><span class="sxs-lookup"><span data-stu-id="f95b1-149">maiden</span></span>        |<span data-ttu-id="f95b1-150">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-150">String</span></span>                                           | <span data-ttu-id="f95b1-151">Sobrenome de casamento do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-151">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="f95b1-152">middleware</span><span class="sxs-lookup"><span data-stu-id="f95b1-152">middle</span></span>        |<span data-ttu-id="f95b1-153">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-153">String</span></span>                                           | <span data-ttu-id="f95b1-154">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-154">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="f95b1-155">apelido</span><span class="sxs-lookup"><span data-stu-id="f95b1-155">nickname</span></span>      |<span data-ttu-id="f95b1-156">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-156">String</span></span>                                           | <span data-ttu-id="f95b1-157">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-157">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="f95b1-158">pronúncia</span><span class="sxs-lookup"><span data-stu-id="f95b1-158">pronunciation</span></span> |[<span data-ttu-id="f95b1-159">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="f95b1-159">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="f95b1-160">Contém detalhes sobre a pronúncia do nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="f95b1-160">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="f95b1-161">sufixo</span><span class="sxs-lookup"><span data-stu-id="f95b1-161">suffix</span></span>        |<span data-ttu-id="f95b1-162">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-162">String</span></span>                                           | <span data-ttu-id="f95b1-163">Designadores usados após o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="f95b1-163">Designators used after the users name.</span></span> <span data-ttu-id="f95b1-164">(por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="f95b1-164">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="f95b1-165">title</span><span class="sxs-lookup"><span data-stu-id="f95b1-165">title</span></span>         |<span data-ttu-id="f95b1-166">String</span><span class="sxs-lookup"><span data-stu-id="f95b1-166">String</span></span>                                           | <span data-ttu-id="f95b1-167">Honorifics usado para prefixar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f95b1-167">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="f95b1-168">(por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="f95b1-168">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="f95b1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95b1-169">Response</span></span>

<span data-ttu-id="f95b1-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [PersonName](../resources/personname.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f95b1-170">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f95b1-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f95b1-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f95b1-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f95b1-172">Request</span></span>

<span data-ttu-id="f95b1-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f95b1-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f95b1-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="f95b1-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f95b1-175">C#</span><span class="sxs-lookup"><span data-stu-id="f95b1-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f95b1-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f95b1-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f95b1-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f95b1-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f95b1-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95b1-178">Response</span></span>

<span data-ttu-id="f95b1-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f95b1-179">The following is an example of the response.</span></span>

> <span data-ttu-id="f95b1-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f95b1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personname",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
