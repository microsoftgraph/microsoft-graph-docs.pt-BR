---
title: Atualizar userAccountInformation
description: Atualize as propriedades do objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78d890a00916c72b8c48e5b41a1c84e1e2e2ffb8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938138"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="bdab8-103">Atualizar useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="bdab8-103">Update useraccountinformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdab8-104">Atualiza as propriedades de um objeto [userAccountInformation](../resources/useraccountinformation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bdab8-104">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdab8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdab8-105">Permissions</span></span>

<span data-ttu-id="bdab8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdab8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdab8-108">Permission type</span></span>                        | <span data-ttu-id="bdab8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdab8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdab8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdab8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdab8-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bdab8-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bdab8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdab8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdab8-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bdab8-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bdab8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdab8-114">Application</span></span>                            | <span data-ttu-id="bdab8-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdab8-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bdab8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdab8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bdab8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdab8-117">Request headers</span></span>

| <span data-ttu-id="bdab8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bdab8-118">Name</span></span>           |<span data-ttu-id="bdab8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdab8-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="bdab8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdab8-120">Authorization</span></span>  | <span data-ttu-id="bdab8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdab8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bdab8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdab8-123">Content-Type</span></span>   | <span data-ttu-id="bdab8-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="bdab8-124">application/json.</span></span> <span data-ttu-id="bdab8-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bdab8-125">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdab8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdab8-126">Request body</span></span>

<span data-ttu-id="bdab8-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bdab8-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bdab8-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bdab8-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bdab8-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bdab8-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bdab8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdab8-130">Property</span></span>            | <span data-ttu-id="bdab8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdab8-131">Type</span></span>                                    | <span data-ttu-id="bdab8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdab8-132">Description</span></span>                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="bdab8-133">ageGroup</span><span class="sxs-lookup"><span data-stu-id="bdab8-133">ageGroup</span></span>             |<span data-ttu-id="bdab8-134">String</span><span class="sxs-lookup"><span data-stu-id="bdab8-134">String</span></span>                                   |<span data-ttu-id="bdab8-135">Mostra o grupo de idade do usuário.</span><span class="sxs-lookup"><span data-stu-id="bdab8-135">Shows the age group of user.</span></span> <span data-ttu-id="bdab8-136">Valores `null`permitidos, `minor` `notAdult` e `adult`.</span><span class="sxs-lookup"><span data-stu-id="bdab8-136">Allowed values `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="bdab8-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdab8-137">Read Only.</span></span> |
|<span data-ttu-id="bdab8-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="bdab8-138">countryCode</span></span>          |<span data-ttu-id="bdab8-139">String</span><span class="sxs-lookup"><span data-stu-id="bdab8-139">String</span></span>                                   |<span data-ttu-id="bdab8-140">Contém os countryCode de dois caracteres associados à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="bdab8-140">Contains the two-character countryCode associated with the users account.</span></span>                       |
|<span data-ttu-id="bdab8-141">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="bdab8-141">preferredLanguageTag</span></span> |[<span data-ttu-id="bdab8-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="bdab8-142">localeInfo</span></span>](../resources/localeinfo.md) |<span data-ttu-id="bdab8-143">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="bdab8-143">Contains the language the user has associated as preferred for the account.</span></span>                     |
|<span data-ttu-id="bdab8-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bdab8-144">userPrincipalName</span></span>    |<span data-ttu-id="bdab8-145">String</span><span class="sxs-lookup"><span data-stu-id="bdab8-145">String</span></span>                                   |<span data-ttu-id="bdab8-146">O nome principal do usuário (UPN) do usuário associado à conta.</span><span class="sxs-lookup"><span data-stu-id="bdab8-146">The user principal name (UPN) of the user associated with the account.</span></span>                          |

## <a name="response"></a><span data-ttu-id="bdab8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdab8-147">Response</span></span>

<span data-ttu-id="bdab8-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userAccountInformation](../resources/useraccountinformation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdab8-148">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdab8-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bdab8-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdab8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdab8-150">Request</span></span>

<span data-ttu-id="bdab8-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdab8-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bdab8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdab8-152">Response</span></span>

<span data-ttu-id="bdab8-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdab8-153">The following is an example of the response.</span></span>

> <span data-ttu-id="bdab8-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdab8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
