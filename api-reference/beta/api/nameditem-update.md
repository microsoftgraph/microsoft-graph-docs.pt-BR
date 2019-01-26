---
title: Atualizar nameditem
description: Atualize as propriedades do objeto nameditem.
localization_priority: Normal
ms.openlocfilehash: b25657a6913a9fe56ce7068b9318fa7390f139f8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577491"
---
# <a name="update-nameditem"></a><span data-ttu-id="cbcd3-103">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="cbcd3-103">Update nameditem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbcd3-104">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbcd3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbcd3-105">Permissions</span></span>
<span data-ttu-id="cbcd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbcd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbcd3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbcd3-108">Permission type</span></span>      | <span data-ttu-id="cbcd3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbcd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbcd3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbcd3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbcd3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbcd3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbcd3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbcd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbcd3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbcd3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbcd3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbcd3-114">Application</span></span> | <span data-ttu-id="cbcd3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbcd3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbcd3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="cbcd3-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cbcd3-117">Optional request headers</span></span>
| <span data-ttu-id="cbcd3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cbcd3-118">Name</span></span>       | <span data-ttu-id="cbcd3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbcd3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cbcd3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbcd3-120">Authorization</span></span>  | <span data-ttu-id="cbcd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbcd3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cbcd3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbcd3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbcd3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbcd3-126">Request body</span></span>
<span data-ttu-id="cbcd3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cbcd3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbcd3-130">Property</span></span>     | <span data-ttu-id="cbcd3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbcd3-131">Type</span></span>   |<span data-ttu-id="cbcd3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbcd3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbcd3-133">visible</span><span class="sxs-lookup"><span data-stu-id="cbcd3-133">visible</span></span>|<span data-ttu-id="cbcd3-134">booliano</span><span class="sxs-lookup"><span data-stu-id="cbcd3-134">boolean</span></span>|<span data-ttu-id="cbcd3-135">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="cbcd3-136">comment</span><span class="sxs-lookup"><span data-stu-id="cbcd3-136">comment</span></span>|   <span data-ttu-id="cbcd3-137">string</span><span class="sxs-lookup"><span data-stu-id="cbcd3-137">string</span></span>  |<span data-ttu-id="cbcd3-138">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="cbcd3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbcd3-139">Response</span></span>

<span data-ttu-id="cbcd3-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-140">If successful, this method returns a `200 OK` response code and updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbcd3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbcd3-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbcd3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbcd3-142">Request</span></span>
<span data-ttu-id="cbcd3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="cbcd3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbcd3-144">Response</span></span>
<span data-ttu-id="cbcd3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbcd3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
