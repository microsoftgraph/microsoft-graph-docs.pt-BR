---
title: Atualizar synchronizationTemplate
description: Atualização (substituição) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: 152186afd9f7b7cce2a04170de7148d454525d80
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517460"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="a7cac-103">Atualizar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="a7cac-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7cac-104">Atualização (substituição) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a7cac-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7cac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7cac-105">Permissions</span></span>
<span data-ttu-id="a7cac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7cac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7cac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7cac-108">Permission type</span></span>                        | <span data-ttu-id="a7cac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7cac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7cac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7cac-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="a7cac-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cac-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a7cac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7cac-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a7cac-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7cac-113">Not supported.</span></span>|
|<span data-ttu-id="a7cac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7cac-114">Application</span></span>                            |<span data-ttu-id="a7cac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7cac-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="a7cac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7cac-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="a7cac-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7cac-117">Request headers</span></span>

| <span data-ttu-id="a7cac-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a7cac-118">Name</span></span>           | <span data-ttu-id="a7cac-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7cac-119">Type</span></span>    | <span data-ttu-id="a7cac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7cac-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a7cac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7cac-121">Authorization</span></span>  | <span data-ttu-id="a7cac-122">string</span><span class="sxs-lookup"><span data-stu-id="a7cac-122">string</span></span>  | <span data-ttu-id="a7cac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7cac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7cac-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7cac-125">Request body</span></span>

<span data-ttu-id="a7cac-126">No corpo da solicitação, fornece o objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="a7cac-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="a7cac-127">Verifique se que todas as propriedades são fornecidas.</span><span class="sxs-lookup"><span data-stu-id="a7cac-127">Make sure all properties are provided.</span></span> <span data-ttu-id="a7cac-128">Propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="a7cac-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="a7cac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7cac-129">Response</span></span>

<span data-ttu-id="a7cac-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7cac-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="a7cac-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7cac-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="a7cac-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7cac-133">Request</span></span>
<span data-ttu-id="a7cac-134">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7cac-134">The following is an example of a request.</span></span> 

><span data-ttu-id="a7cac-135">**Observação:** O objeto request mostrado aqui é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a7cac-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="a7cac-136">Inclua todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7cac-136">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="a7cac-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7cac-137">Response</span></span>
<span data-ttu-id="a7cac-138">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a7cac-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
