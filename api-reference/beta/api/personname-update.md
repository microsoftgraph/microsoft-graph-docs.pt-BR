---
title: Atualizar PersonName
description: Atualiza as propriedades de um objeto PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 97a4497b88e7cb065ea5ad73229dc4acc8c45556
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937858"
---
# <a name="update-personname"></a><span data-ttu-id="a520d-103">Atualizar PersonName</span><span class="sxs-lookup"><span data-stu-id="a520d-103">Update personname</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a520d-104">Atualiza as propriedades de um objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-104">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a520d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a520d-105">Permissions</span></span>

<span data-ttu-id="a520d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a520d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a520d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a520d-108">Permission type</span></span>                        | <span data-ttu-id="a520d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a520d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a520d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a520d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a520d-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a520d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a520d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a520d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a520d-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a520d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a520d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a520d-114">Application</span></span>                            | <span data-ttu-id="a520d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a520d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a520d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a520d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a520d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a520d-117">Request headers</span></span>

| <span data-ttu-id="a520d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a520d-118">Name</span></span>           |<span data-ttu-id="a520d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a520d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a520d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a520d-120">Authorization</span></span>  | <span data-ttu-id="a520d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a520d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a520d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a520d-123">Content-Type</span></span>   | <span data-ttu-id="a520d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a520d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a520d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a520d-126">Request body</span></span>

<span data-ttu-id="a520d-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a520d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a520d-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a520d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a520d-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a520d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a520d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a520d-130">Property</span></span>     | <span data-ttu-id="a520d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a520d-131">Type</span></span>                                            | <span data-ttu-id="a520d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a520d-132">Description</span></span>                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="a520d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a520d-133">displayName</span></span>   |<span data-ttu-id="a520d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a520d-134">String</span></span>                                           | <span data-ttu-id="a520d-135">Fornece um processamento ordenado de nome e sobrenome.</span><span class="sxs-lookup"><span data-stu-id="a520d-135">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="a520d-136">primeiro</span><span class="sxs-lookup"><span data-stu-id="a520d-136">first</span></span>         |<span data-ttu-id="a520d-137">String</span><span class="sxs-lookup"><span data-stu-id="a520d-137">String</span></span>                                           | <span data-ttu-id="a520d-138">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-138">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="a520d-139">initials</span><span class="sxs-lookup"><span data-stu-id="a520d-139">initials</span></span>      |<span data-ttu-id="a520d-140">String</span><span class="sxs-lookup"><span data-stu-id="a520d-140">String</span></span>                                           | <span data-ttu-id="a520d-141">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-141">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="a520d-142">languageTag</span><span class="sxs-lookup"><span data-stu-id="a520d-142">languageTag</span></span>   |<span data-ttu-id="a520d-143">String</span><span class="sxs-lookup"><span data-stu-id="a520d-143">String</span></span>                                           | <span data-ttu-id="a520d-144">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="a520d-144">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="a520d-145">durar</span><span class="sxs-lookup"><span data-stu-id="a520d-145">last</span></span>          |<span data-ttu-id="a520d-146">String</span><span class="sxs-lookup"><span data-stu-id="a520d-146">String</span></span>                                           | <span data-ttu-id="a520d-147">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-147">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="a520d-148">Virgem</span><span class="sxs-lookup"><span data-stu-id="a520d-148">maiden</span></span>        |<span data-ttu-id="a520d-149">String</span><span class="sxs-lookup"><span data-stu-id="a520d-149">String</span></span>                                           | <span data-ttu-id="a520d-150">Sobrenome de casamento do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-150">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="a520d-151">middleware</span><span class="sxs-lookup"><span data-stu-id="a520d-151">middle</span></span>        |<span data-ttu-id="a520d-152">String</span><span class="sxs-lookup"><span data-stu-id="a520d-152">String</span></span>                                           | <span data-ttu-id="a520d-153">Nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-153">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="a520d-154">apelido</span><span class="sxs-lookup"><span data-stu-id="a520d-154">nickname</span></span>      |<span data-ttu-id="a520d-155">String</span><span class="sxs-lookup"><span data-stu-id="a520d-155">String</span></span>                                           | <span data-ttu-id="a520d-156">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-156">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="a520d-157">pronúncia</span><span class="sxs-lookup"><span data-stu-id="a520d-157">pronunciation</span></span> |[<span data-ttu-id="a520d-158">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="a520d-158">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="a520d-159">Contém detalhes sobre a pronúncia do nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="a520d-159">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="a520d-160">sufixo</span><span class="sxs-lookup"><span data-stu-id="a520d-160">suffix</span></span>        |<span data-ttu-id="a520d-161">String</span><span class="sxs-lookup"><span data-stu-id="a520d-161">String</span></span>                                           | <span data-ttu-id="a520d-162">Designadores usados após o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="a520d-162">Designators used after the users name.</span></span> <span data-ttu-id="a520d-163">(por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="a520d-163">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="a520d-164">title</span><span class="sxs-lookup"><span data-stu-id="a520d-164">title</span></span>         |<span data-ttu-id="a520d-165">String</span><span class="sxs-lookup"><span data-stu-id="a520d-165">String</span></span>                                           | <span data-ttu-id="a520d-166">Honorifics usado para prefixar um nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="a520d-166">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="a520d-167">(por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="a520d-167">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="a520d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a520d-168">Response</span></span>

<span data-ttu-id="a520d-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [PersonName](../resources/personname.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a520d-169">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a520d-170">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a520d-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a520d-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a520d-171">Request</span></span>

<span data-ttu-id="a520d-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a520d-172">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a520d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a520d-173">Response</span></span>

<span data-ttu-id="a520d-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a520d-174">The following is an example of the response.</span></span>

> <span data-ttu-id="a520d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a520d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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