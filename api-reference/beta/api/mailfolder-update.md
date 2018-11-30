---
title: Atualizar mailFolder
description: Atualize as propriedades do objeto mailFolder.
ms.openlocfilehash: 13851d4d538083658abd6ddba7d9368071b5372e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037063"
---
# <a name="update-mailfolder"></a><span data-ttu-id="4bcb3-103">Atualizar mailFolder</span><span class="sxs-lookup"><span data-stu-id="4bcb3-103">Update mailFolder</span></span>

> <span data-ttu-id="4bcb3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bcb3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bcb3-106">Atualize as propriedades do objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="4bcb3-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bcb3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4bcb3-107">Permissions</span></span>
<span data-ttu-id="4bcb3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bcb3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bcb3-110">Permission type</span></span>      | <span data-ttu-id="4bcb3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bcb3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bcb3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bcb3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4bcb3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bcb3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bcb3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4bcb3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bcb3-116">Application</span></span> | <span data-ttu-id="4bcb3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bcb3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bcb3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bcb3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4bcb3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bcb3-119">Request headers</span></span>
| <span data-ttu-id="4bcb3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bcb3-120">Header</span></span>       | <span data-ttu-id="4bcb3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bcb3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4bcb3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bcb3-122">Authorization</span></span>  | <span data-ttu-id="4bcb3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4bcb3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bcb3-125">Content-Type</span></span>  | <span data-ttu-id="4bcb3-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4bcb3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bcb3-128">Request body</span></span>
<span data-ttu-id="4bcb3-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4bcb3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bcb3-132">Property</span></span>     | <span data-ttu-id="4bcb3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bcb3-133">Type</span></span>   |<span data-ttu-id="4bcb3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bcb3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bcb3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4bcb3-135">displayName</span></span>|<span data-ttu-id="4bcb3-136">String</span><span class="sxs-lookup"><span data-stu-id="4bcb3-136">String</span></span>|<span data-ttu-id="4bcb3-137">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="4bcb3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bcb3-138">Response</span></span>
<span data-ttu-id="4bcb3-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bcb3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bcb3-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4bcb3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bcb3-141">Request</span></span>
<span data-ttu-id="4bcb3-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="4bcb3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bcb3-143">Response</span></span>
<span data-ttu-id="4bcb3-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-144">The following is an example of the response.</span></span>
><span data-ttu-id="4bcb3-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4bcb3-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bcb3-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
