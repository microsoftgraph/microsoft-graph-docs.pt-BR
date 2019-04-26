---
title: Atualizar mailFolder
description: Atualize as propriedades do objeto mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0c1a9ee3d4314ede96072b39e00e29dc15d6be84
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338611"
---
# <a name="update-mailfolder"></a><span data-ttu-id="9f9a5-103">Atualizar mailFolder</span><span class="sxs-lookup"><span data-stu-id="9f9a5-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f9a5-104">Atualize as propriedades do objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="9f9a5-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f9a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f9a5-105">Permissions</span></span>
<span data-ttu-id="9f9a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f9a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f9a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f9a5-108">Permission type</span></span>      | <span data-ttu-id="9f9a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f9a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f9a5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f9a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f9a5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f9a5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f9a5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f9a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f9a5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f9a5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f9a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f9a5-114">Application</span></span> | <span data-ttu-id="9f9a5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f9a5-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f9a5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f9a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f9a5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f9a5-117">Request headers</span></span>
| <span data-ttu-id="9f9a5-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f9a5-118">Header</span></span>       | <span data-ttu-id="9f9a5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9f9a5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f9a5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f9a5-120">Authorization</span></span>  | <span data-ttu-id="9f9a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f9a5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f9a5-123">Content-Type</span></span>  | <span data-ttu-id="9f9a5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f9a5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f9a5-126">Request body</span></span>
<span data-ttu-id="9f9a5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f9a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f9a5-130">Property</span></span>     | <span data-ttu-id="9f9a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f9a5-131">Type</span></span>   |<span data-ttu-id="9f9a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f9a5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f9a5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9a5-133">displayName</span></span>|<span data-ttu-id="9f9a5-134">String</span><span class="sxs-lookup"><span data-stu-id="9f9a5-134">String</span></span>|<span data-ttu-id="9f9a5-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="9f9a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f9a5-136">Response</span></span>
<span data-ttu-id="9f9a5-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f9a5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f9a5-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9f9a5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f9a5-139">Request</span></span>
<span data-ttu-id="9f9a5-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-140">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9f9a5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f9a5-141">Response</span></span>
<span data-ttu-id="9f9a5-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-142">The following is an example of the response.</span></span>
><span data-ttu-id="9f9a5-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f9a5-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f9a5-144">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
