---
title: Atualizar PersonName
description: Atualiza as propriedades de um objeto PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f288d73956b79c0ab5c47524239069f2c239791c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997204"
---
# <a name="update-personname"></a><span data-ttu-id="335ba-103">Atualizar PersonName</span><span class="sxs-lookup"><span data-stu-id="335ba-103">Update personname</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="335ba-104">Atualiza as propriedades de um objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-104">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="335ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="335ba-105">Permissions</span></span>

<span data-ttu-id="335ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="335ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="335ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="335ba-108">Permission type</span></span>                        | <span data-ttu-id="335ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="335ba-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="335ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="335ba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="335ba-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="335ba-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="335ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="335ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="335ba-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="335ba-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="335ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="335ba-114">Application</span></span>                            | <span data-ttu-id="335ba-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="335ba-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="335ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="335ba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="335ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="335ba-117">Request headers</span></span>

| <span data-ttu-id="335ba-118">Nome</span><span class="sxs-lookup"><span data-stu-id="335ba-118">Name</span></span>           |<span data-ttu-id="335ba-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="335ba-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="335ba-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="335ba-120">Authorization</span></span>  | <span data-ttu-id="335ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="335ba-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="335ba-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="335ba-123">Content-Type</span></span>   | <span data-ttu-id="335ba-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="335ba-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="335ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="335ba-126">Request body</span></span>

<span data-ttu-id="335ba-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="335ba-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="335ba-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="335ba-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="335ba-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="335ba-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="335ba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="335ba-130">Property</span></span>     | <span data-ttu-id="335ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="335ba-131">Type</span></span>                                            | <span data-ttu-id="335ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="335ba-132">Description</span></span>                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="335ba-133">displayName</span><span class="sxs-lookup"><span data-stu-id="335ba-133">displayName</span></span>   |<span data-ttu-id="335ba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="335ba-134">String</span></span>                                           | <span data-ttu-id="335ba-135">Fornece um processamento ordenado de nome e sobrenome.</span><span class="sxs-lookup"><span data-stu-id="335ba-135">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="335ba-136">primeiro</span><span class="sxs-lookup"><span data-stu-id="335ba-136">first</span></span>         |<span data-ttu-id="335ba-137">String</span><span class="sxs-lookup"><span data-stu-id="335ba-137">String</span></span>                                           | <span data-ttu-id="335ba-138">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-138">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="335ba-139">initials</span><span class="sxs-lookup"><span data-stu-id="335ba-139">initials</span></span>      |<span data-ttu-id="335ba-140">String</span><span class="sxs-lookup"><span data-stu-id="335ba-140">String</span></span>                                           | <span data-ttu-id="335ba-141">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-141">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="335ba-142">languageTag</span><span class="sxs-lookup"><span data-stu-id="335ba-142">languageTag</span></span>   |<span data-ttu-id="335ba-143">String</span><span class="sxs-lookup"><span data-stu-id="335ba-143">String</span></span>                                           | <span data-ttu-id="335ba-144">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="335ba-144">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="335ba-145">durar</span><span class="sxs-lookup"><span data-stu-id="335ba-145">last</span></span>          |<span data-ttu-id="335ba-146">String</span><span class="sxs-lookup"><span data-stu-id="335ba-146">String</span></span>                                           | <span data-ttu-id="335ba-147">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-147">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="335ba-148">Virgem</span><span class="sxs-lookup"><span data-stu-id="335ba-148">maiden</span></span>        |<span data-ttu-id="335ba-149">String</span><span class="sxs-lookup"><span data-stu-id="335ba-149">String</span></span>                                           | <span data-ttu-id="335ba-150">Sobrenome de casamento do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-150">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="335ba-151">middleware</span><span class="sxs-lookup"><span data-stu-id="335ba-151">middle</span></span>        |<span data-ttu-id="335ba-152">String</span><span class="sxs-lookup"><span data-stu-id="335ba-152">String</span></span>                                           | <span data-ttu-id="335ba-153">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-153">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="335ba-154">apelido</span><span class="sxs-lookup"><span data-stu-id="335ba-154">nickname</span></span>      |<span data-ttu-id="335ba-155">String</span><span class="sxs-lookup"><span data-stu-id="335ba-155">String</span></span>                                           | <span data-ttu-id="335ba-156">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-156">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="335ba-157">pronúncia</span><span class="sxs-lookup"><span data-stu-id="335ba-157">pronunciation</span></span> |[<span data-ttu-id="335ba-158">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="335ba-158">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="335ba-159">Contém detalhes sobre a pronúncia do nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="335ba-159">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="335ba-160">sufixo</span><span class="sxs-lookup"><span data-stu-id="335ba-160">suffix</span></span>        |<span data-ttu-id="335ba-161">String</span><span class="sxs-lookup"><span data-stu-id="335ba-161">String</span></span>                                           | <span data-ttu-id="335ba-162">Designadores usados após o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="335ba-162">Designators used after the users name.</span></span> <span data-ttu-id="335ba-163">(por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="335ba-163">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="335ba-164">title</span><span class="sxs-lookup"><span data-stu-id="335ba-164">title</span></span>         |<span data-ttu-id="335ba-165">String</span><span class="sxs-lookup"><span data-stu-id="335ba-165">String</span></span>                                           | <span data-ttu-id="335ba-166">Honorifics usado para prefixar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="335ba-166">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="335ba-167">(por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="335ba-167">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="335ba-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="335ba-168">Response</span></span>

<span data-ttu-id="335ba-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [PersonName](../resources/personname.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="335ba-169">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="335ba-170">Exemplos</span><span class="sxs-lookup"><span data-stu-id="335ba-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="335ba-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="335ba-171">Request</span></span>

<span data-ttu-id="335ba-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="335ba-172">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="335ba-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="335ba-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="335ba-174">C#</span><span class="sxs-lookup"><span data-stu-id="335ba-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="335ba-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="335ba-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="335ba-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="335ba-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="335ba-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="335ba-177">Response</span></span>

<span data-ttu-id="335ba-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="335ba-178">The following is an example of the response.</span></span>

> <span data-ttu-id="335ba-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="335ba-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
