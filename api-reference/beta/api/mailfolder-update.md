---
title: Atualizar mailfolder
description: Atualizar as propriedades do objeto de mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 63642678a58271bd0c0218879bf22504842c11e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518111"
---
# <a name="update-mailfolder"></a><span data-ttu-id="9093d-103">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="9093d-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9093d-104">Atualizar as propriedades do objeto de mailfolder.</span><span class="sxs-lookup"><span data-stu-id="9093d-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9093d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9093d-105">Permissions</span></span>
<span data-ttu-id="9093d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9093d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9093d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9093d-108">Permission type</span></span>      | <span data-ttu-id="9093d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9093d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9093d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9093d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9093d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9093d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9093d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9093d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9093d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9093d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9093d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9093d-114">Application</span></span> | <span data-ttu-id="9093d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9093d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9093d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9093d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9093d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9093d-117">Request headers</span></span>
| <span data-ttu-id="9093d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9093d-118">Header</span></span>       | <span data-ttu-id="9093d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9093d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9093d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9093d-120">Authorization</span></span>  | <span data-ttu-id="9093d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9093d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9093d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9093d-123">Content-Type</span></span>  | <span data-ttu-id="9093d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9093d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9093d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9093d-126">Request body</span></span>
<span data-ttu-id="9093d-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9093d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9093d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9093d-130">Property</span></span>     | <span data-ttu-id="9093d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9093d-131">Type</span></span>   |<span data-ttu-id="9093d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9093d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9093d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9093d-133">displayName</span></span>|<span data-ttu-id="9093d-134">String</span><span class="sxs-lookup"><span data-stu-id="9093d-134">String</span></span>|<span data-ttu-id="9093d-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="9093d-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="9093d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9093d-136">Response</span></span>
<span data-ttu-id="9093d-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9093d-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9093d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9093d-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9093d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9093d-139">Request</span></span>
<span data-ttu-id="9093d-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9093d-140">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9093d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9093d-141">Response</span></span>
<span data-ttu-id="9093d-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9093d-142">The following is an example of the response.</span></span>
><span data-ttu-id="9093d-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9093d-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9093d-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9093d-144">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
