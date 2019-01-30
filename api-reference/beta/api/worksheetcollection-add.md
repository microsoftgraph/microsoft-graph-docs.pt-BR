---
title: 'WorksheetCollection: add'
description: .Activate() nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0958f8f82502c92eff08ec80a7b116c1b0c4a5f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640837"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="b9a3d-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="b9a3d-103">WorksheetCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a3d-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9a3d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9a3d-107">Permissions</span></span>
<span data-ttu-id="b9a3d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a3d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a3d-110">Permission type</span></span>      | <span data-ttu-id="b9a3d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9a3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a3d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a3d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a3d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9a3d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a3d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a3d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9a3d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a3d-116">Application</span></span> | <span data-ttu-id="b9a3d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a3d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="b9a3d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a3d-119">Request headers</span></span>
| <span data-ttu-id="b9a3d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b9a3d-120">Name</span></span>       | <span data-ttu-id="b9a3d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a3d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9a3d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a3d-122">Authorization</span></span>  | <span data-ttu-id="b9a3d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9a3d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9a3d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9a3d-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a3d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a3d-128">Request body</span></span>
<span data-ttu-id="b9a3d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9a3d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9a3d-130">Parameter</span></span>    | <span data-ttu-id="b9a3d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a3d-131">Type</span></span>   |<span data-ttu-id="b9a3d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a3d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9a3d-133">name</span><span class="sxs-lookup"><span data-stu-id="b9a3d-133">name</span></span>|<span data-ttu-id="b9a3d-134">string</span><span class="sxs-lookup"><span data-stu-id="b9a3d-134">string</span></span>|<span data-ttu-id="b9a3d-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="b9a3d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a3d-139">Response</span></span>

<span data-ttu-id="b9a3d-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-140">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a3d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a3d-141">Example</span></span>
<span data-ttu-id="b9a3d-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9a3d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a3d-143">Request</span></span>
<span data-ttu-id="b9a3d-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="b9a3d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a3d-145">Response</span></span>
<span data-ttu-id="b9a3d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9a3d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
