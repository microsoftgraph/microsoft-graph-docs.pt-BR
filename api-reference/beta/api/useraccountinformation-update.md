---
title: Atualizar userAccountInformation
description: Atualize as propriedades do objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 429e26ef14ed461c61f00072cdad878f59d5870f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451593"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="f0491-103">Atualizar useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="f0491-103">Update useraccountinformation</span></span>

<span data-ttu-id="f0491-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0491-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0491-105">Atualiza as propriedades de um objeto [userAccountInformation](../resources/useraccountinformation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f0491-105">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0491-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0491-106">Permissions</span></span>

<span data-ttu-id="f0491-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0491-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0491-109">Permission type</span></span>                        | <span data-ttu-id="f0491-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0491-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0491-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0491-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0491-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0491-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f0491-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0491-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0491-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0491-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f0491-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0491-115">Application</span></span>                            | <span data-ttu-id="f0491-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0491-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f0491-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0491-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0491-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0491-118">Request headers</span></span>

| <span data-ttu-id="f0491-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f0491-119">Name</span></span>           |<span data-ttu-id="f0491-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0491-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="f0491-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0491-121">Authorization</span></span>  | <span data-ttu-id="f0491-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0491-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0491-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0491-124">Content-Type</span></span>   | <span data-ttu-id="f0491-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="f0491-125">application/json.</span></span> <span data-ttu-id="f0491-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f0491-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0491-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0491-127">Request body</span></span>

<span data-ttu-id="f0491-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f0491-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f0491-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f0491-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f0491-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f0491-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0491-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0491-131">Property</span></span>            | <span data-ttu-id="f0491-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0491-132">Type</span></span>                                    | <span data-ttu-id="f0491-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0491-133">Description</span></span>                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="f0491-134">ageGroup</span><span class="sxs-lookup"><span data-stu-id="f0491-134">ageGroup</span></span>             |<span data-ttu-id="f0491-135">String</span><span class="sxs-lookup"><span data-stu-id="f0491-135">String</span></span>                                   |<span data-ttu-id="f0491-136">Mostra o grupo de idade do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0491-136">Shows the age group of user.</span></span> <span data-ttu-id="f0491-137">Valores `null`permitidos, `minor` `notAdult` e `adult`.</span><span class="sxs-lookup"><span data-stu-id="f0491-137">Allowed values `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="f0491-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0491-138">Read Only.</span></span> |
|<span data-ttu-id="f0491-139">countryCode</span><span class="sxs-lookup"><span data-stu-id="f0491-139">countryCode</span></span>          |<span data-ttu-id="f0491-140">String</span><span class="sxs-lookup"><span data-stu-id="f0491-140">String</span></span>                                   |<span data-ttu-id="f0491-141">Contém os countryCode de dois caracteres associados à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="f0491-141">Contains the two-character countryCode associated with the users account.</span></span>                       |
|<span data-ttu-id="f0491-142">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="f0491-142">preferredLanguageTag</span></span> |[<span data-ttu-id="f0491-143">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f0491-143">localeInfo</span></span>](../resources/localeinfo.md) |<span data-ttu-id="f0491-144">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="f0491-144">Contains the language the user has associated as preferred for the account.</span></span>                     |
|<span data-ttu-id="f0491-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0491-145">userPrincipalName</span></span>    |<span data-ttu-id="f0491-146">String</span><span class="sxs-lookup"><span data-stu-id="f0491-146">String</span></span>                                   |<span data-ttu-id="f0491-147">O nome principal do usuário (UPN) do usuário associado à conta.</span><span class="sxs-lookup"><span data-stu-id="f0491-147">The user principal name (UPN) of the user associated with the account.</span></span>                          |

## <a name="response"></a><span data-ttu-id="f0491-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0491-148">Response</span></span>

<span data-ttu-id="f0491-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userAccountInformation](../resources/useraccountinformation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0491-149">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0491-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0491-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0491-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0491-151">Request</span></span>

<span data-ttu-id="f0491-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0491-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0491-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0491-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f0491-154">C#</span><span class="sxs-lookup"><span data-stu-id="f0491-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0491-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0491-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0491-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0491-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0491-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0491-157">Response</span></span>

<span data-ttu-id="f0491-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0491-158">The following is an example of the response.</span></span>

> <span data-ttu-id="f0491-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0491-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update useraccountinformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
