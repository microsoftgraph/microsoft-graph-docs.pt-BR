---
title: 'WorksheetCollection: add'
description: .Activate() nele.
ms.openlocfilehash: 992524aae6dfca0619c043eb0ddb7a4100f50206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005027"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="69d57-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="69d57-103">WorksheetCollection: add</span></span>

<span data-ttu-id="69d57-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="69d57-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="69d57-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="69d57-107">Permissions</span></span>
<span data-ttu-id="69d57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69d57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69d57-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69d57-110">Permission type</span></span>      | <span data-ttu-id="69d57-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69d57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69d57-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69d57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69d57-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69d57-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69d57-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69d57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69d57-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69d57-115">Not supported.</span></span>    |
|<span data-ttu-id="69d57-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69d57-116">Application</span></span> | <span data-ttu-id="69d57-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69d57-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69d57-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69d57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="69d57-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69d57-119">Request headers</span></span>
| <span data-ttu-id="69d57-120">Nome</span><span class="sxs-lookup"><span data-stu-id="69d57-120">Name</span></span>       | <span data-ttu-id="69d57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="69d57-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69d57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69d57-122">Authorization</span></span>  | <span data-ttu-id="69d57-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69d57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69d57-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="69d57-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="69d57-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="69d57-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69d57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69d57-128">Request body</span></span>
<span data-ttu-id="69d57-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69d57-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69d57-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="69d57-130">Parameter</span></span>    | <span data-ttu-id="69d57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69d57-131">Type</span></span>   |<span data-ttu-id="69d57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69d57-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69d57-133">name</span><span class="sxs-lookup"><span data-stu-id="69d57-133">name</span></span>|<span data-ttu-id="69d57-134">string</span><span class="sxs-lookup"><span data-stu-id="69d57-134">string</span></span>|<span data-ttu-id="69d57-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="69d57-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="69d57-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="69d57-139">Response</span></span>

<span data-ttu-id="69d57-140">Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69d57-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69d57-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69d57-141">Example</span></span>
<span data-ttu-id="69d57-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="69d57-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="69d57-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69d57-143">Request</span></span>
<span data-ttu-id="69d57-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69d57-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="69d57-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="69d57-145">Response</span></span>
<span data-ttu-id="69d57-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69d57-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->