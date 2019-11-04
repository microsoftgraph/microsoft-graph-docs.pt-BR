---
title: Atualizar webaccount
description: Atualizar as propriedades de um objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 93378ab41227ca43457fff2b41a27f7ed07bb0f1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938124"
---
# <a name="update-webaccount"></a><span data-ttu-id="0440d-103">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="0440d-103">Update webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0440d-104">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0440d-104">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0440d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0440d-105">Permissions</span></span>

<span data-ttu-id="0440d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0440d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0440d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0440d-108">Permission type</span></span>                        | <span data-ttu-id="0440d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0440d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0440d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0440d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0440d-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0440d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0440d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0440d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0440d-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0440d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0440d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0440d-114">Application</span></span>                            | <span data-ttu-id="0440d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0440d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0440d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0440d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0440d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0440d-117">Request headers</span></span>

| <span data-ttu-id="0440d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0440d-118">Name</span></span>           |<span data-ttu-id="0440d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0440d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0440d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0440d-120">Authorization</span></span>  | <span data-ttu-id="0440d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0440d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0440d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0440d-123">Content-Type</span></span>   | <span data-ttu-id="0440d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0440d-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0440d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0440d-126">Request body</span></span>

<span data-ttu-id="0440d-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0440d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0440d-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0440d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0440d-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0440d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0440d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0440d-130">Property</span></span>     | <span data-ttu-id="0440d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0440d-131">Type</span></span>                                                    | <span data-ttu-id="0440d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0440d-132">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0440d-133">description</span><span class="sxs-lookup"><span data-stu-id="0440d-133">description</span></span>   |<span data-ttu-id="0440d-134">String</span><span class="sxs-lookup"><span data-stu-id="0440d-134">String</span></span>                                                   | <span data-ttu-id="0440d-135">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="0440d-135">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="0440d-136">service</span><span class="sxs-lookup"><span data-stu-id="0440d-136">service</span></span>       |[<span data-ttu-id="0440d-137">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="0440d-137">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="0440d-138">Representa os dados descritivos básicos sobre o serviço de nuvem fornecido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="0440d-138">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="0440d-139">statusMessage</span><span class="sxs-lookup"><span data-stu-id="0440d-139">statusMessage</span></span> |<span data-ttu-id="0440d-140">String</span><span class="sxs-lookup"><span data-stu-id="0440d-140">String</span></span>                                                   | <span data-ttu-id="0440d-141">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="0440d-141">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="0440d-142">userId</span><span class="sxs-lookup"><span data-stu-id="0440d-142">userId</span></span>        |<span data-ttu-id="0440d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0440d-143">String</span></span>                                                   | <span data-ttu-id="0440d-144">O nome de usuário exibido para a conta da webaccount (por exemplo, @kevinb).</span><span class="sxs-lookup"><span data-stu-id="0440d-144">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                                       |
|<span data-ttu-id="0440d-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="0440d-145">webUrl</span></span>        |<span data-ttu-id="0440d-146">String</span><span class="sxs-lookup"><span data-stu-id="0440d-146">String</span></span>                                                   | <span data-ttu-id="0440d-147">Contém um link para o perfil de usuários no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="0440d-147">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="0440d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0440d-148">Response</span></span>

<span data-ttu-id="0440d-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [webaccount](../resources/webaccount.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0440d-149">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0440d-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0440d-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0440d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0440d-151">Request</span></span>

<span data-ttu-id="0440d-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0440d-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="0440d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0440d-153">Response</span></span>

<span data-ttu-id="0440d-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0440d-154">The following is an example of the response.</span></span>

> <span data-ttu-id="0440d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0440d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update webaccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
