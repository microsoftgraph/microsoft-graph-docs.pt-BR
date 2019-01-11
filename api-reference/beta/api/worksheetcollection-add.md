---
title: 'WorksheetCollection: add'
description: .Activate() nele.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: df5cf2fcdd406802e370fc292480fc012cbc6e8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882758"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="eaf8d-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="eaf8d-103">WorksheetCollection: add</span></span>

> <span data-ttu-id="eaf8d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaf8d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaf8d-p102">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p102">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaf8d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaf8d-109">Permissions</span></span>
<span data-ttu-id="eaf8d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf8d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaf8d-112">Permission type</span></span>      | <span data-ttu-id="eaf8d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaf8d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaf8d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaf8d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eaf8d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaf8d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eaf8d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaf8d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaf8d-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaf8d-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eaf8d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaf8d-118">Application</span></span> | <span data-ttu-id="eaf8d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaf8d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaf8d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="eaf8d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf8d-121">Request headers</span></span>
| <span data-ttu-id="eaf8d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="eaf8d-122">Name</span></span>       | <span data-ttu-id="eaf8d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf8d-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eaf8d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaf8d-124">Authorization</span></span>  | <span data-ttu-id="eaf8d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eaf8d-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eaf8d-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="eaf8d-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf8d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf8d-130">Request body</span></span>
<span data-ttu-id="eaf8d-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eaf8d-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eaf8d-132">Parameter</span></span>    | <span data-ttu-id="eaf8d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf8d-133">Type</span></span>   |<span data-ttu-id="eaf8d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf8d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaf8d-135">name</span><span class="sxs-lookup"><span data-stu-id="eaf8d-135">name</span></span>|<span data-ttu-id="eaf8d-136">string</span><span class="sxs-lookup"><span data-stu-id="eaf8d-136">string</span></span>|<span data-ttu-id="eaf8d-p106">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p106">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="eaf8d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf8d-141">Response</span></span>

<span data-ttu-id="eaf8d-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-142">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf8d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaf8d-143">Example</span></span>
<span data-ttu-id="eaf8d-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eaf8d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf8d-145">Request</span></span>
<span data-ttu-id="eaf8d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eaf8d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf8d-147">Response</span></span>
<span data-ttu-id="eaf8d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaf8d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
