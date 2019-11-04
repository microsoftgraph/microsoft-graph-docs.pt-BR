---
title: Atualizar o número de telefone
description: Atualiza as propriedades de um objeto MyPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16c50b41e0c8a5993433b98bf394d22379ae04bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938075"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="f94e6-103">Atualizar itemphonenumber</span><span class="sxs-lookup"><span data-stu-id="f94e6-103">Update itemphonenumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f94e6-104">Atualizar as propriedades de um objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f94e6-104">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f94e6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f94e6-105">Permissions</span></span>

<span data-ttu-id="f94e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f94e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f94e6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f94e6-108">Permission type</span></span>                        | <span data-ttu-id="f94e6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f94e6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f94e6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f94e6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f94e6-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f94e6-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f94e6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f94e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94e6-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f94e6-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f94e6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f94e6-114">Application</span></span>                            | <span data-ttu-id="f94e6-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94e6-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f94e6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f94e6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="f94e6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f94e6-117">Request headers</span></span>

| <span data-ttu-id="f94e6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f94e6-118">Name</span></span>           |<span data-ttu-id="f94e6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f94e6-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f94e6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f94e6-120">Authorization</span></span>  | <span data-ttu-id="f94e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f94e6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f94e6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f94e6-123">Content-Type</span></span>   | <span data-ttu-id="f94e6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f94e6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f94e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f94e6-126">Request body</span></span>

<span data-ttu-id="f94e6-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f94e6-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f94e6-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f94e6-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f94e6-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f94e6-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f94e6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f94e6-130">Property</span></span>     | <span data-ttu-id="f94e6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f94e6-131">Type</span></span>        | <span data-ttu-id="f94e6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f94e6-132">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f94e6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f94e6-133">displayName</span></span>   |<span data-ttu-id="f94e6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f94e6-134">String</span></span>       | <span data-ttu-id="f94e6-135">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="f94e6-135">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="f94e6-136">number</span><span class="sxs-lookup"><span data-stu-id="f94e6-136">number</span></span>        |<span data-ttu-id="f94e6-137">String</span><span class="sxs-lookup"><span data-stu-id="f94e6-137">String</span></span>       | <span data-ttu-id="f94e6-138">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="f94e6-138">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="f94e6-139">type</span><span class="sxs-lookup"><span data-stu-id="f94e6-139">type</span></span>          |<span data-ttu-id="f94e6-140">string</span><span class="sxs-lookup"><span data-stu-id="f94e6-140">string</span></span>       | <span data-ttu-id="f94e6-141">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="f94e6-141">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="f94e6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94e6-142">Response</span></span>

<span data-ttu-id="f94e6-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [MyPhone](../resources/itemphone.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f94e6-143">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f94e6-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f94e6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f94e6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f94e6-145">Request</span></span>

<span data-ttu-id="f94e6-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f94e6-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/phones/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

### <a name="response"></a><span data-ttu-id="f94e6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94e6-147">Response</span></span>

<span data-ttu-id="f94e6-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f94e6-148">The following is an example of the response.</span></span>

> <span data-ttu-id="f94e6-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f94e6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itemphone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->