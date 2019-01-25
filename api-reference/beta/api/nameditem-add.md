---
title: Adicionar Item nomeado
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
ms.openlocfilehash: dd35f2ded1c08c5f6b99a017b89dd6b5b50026b7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525259"
---
# <a name="add-named-item"></a><span data-ttu-id="8ff54-103">Adicionar Item nomeado</span><span class="sxs-lookup"><span data-stu-id="8ff54-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff54-104">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="8ff54-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff54-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ff54-105">Permissions</span></span>
<span data-ttu-id="8ff54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff54-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff54-108">Permission type</span></span>      | <span data-ttu-id="8ff54-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff54-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff54-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ff54-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="8ff54-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff54-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff54-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ff54-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff54-114">Application</span></span> | <span data-ttu-id="8ff54-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ff54-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff54-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="8ff54-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff54-117">Request headers</span></span>
| <span data-ttu-id="8ff54-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ff54-118">Name</span></span>       | <span data-ttu-id="8ff54-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff54-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ff54-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff54-120">Authorization</span></span>  | <span data-ttu-id="8ff54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff54-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ff54-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ff54-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ff54-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ff54-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff54-126">Request body</span></span>
<span data-ttu-id="8ff54-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff54-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ff54-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8ff54-128">Parameter</span></span>    | <span data-ttu-id="8ff54-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff54-129">Type</span></span>   |<span data-ttu-id="8ff54-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff54-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ff54-131">name</span><span class="sxs-lookup"><span data-stu-id="8ff54-131">name</span></span>|<span data-ttu-id="8ff54-132">string</span><span class="sxs-lookup"><span data-stu-id="8ff54-132">string</span></span>|<span data-ttu-id="8ff54-133">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="8ff54-133">The name of the named item.</span></span>|
|<span data-ttu-id="8ff54-134">reference</span><span class="sxs-lookup"><span data-stu-id="8ff54-134">reference</span></span>|<span data-ttu-id="8ff54-135">string</span><span class="sxs-lookup"><span data-stu-id="8ff54-135">string</span></span>|<span data-ttu-id="8ff54-136">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="8ff54-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="8ff54-137">comentário</span><span class="sxs-lookup"><span data-stu-id="8ff54-137">comment</span></span>|<span data-ttu-id="8ff54-138">string</span><span class="sxs-lookup"><span data-stu-id="8ff54-138">string</span></span>|<span data-ttu-id="8ff54-139">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="8ff54-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="8ff54-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff54-140">Response</span></span>

<span data-ttu-id="8ff54-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [NamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff54-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff54-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff54-142">Example</span></span>
<span data-ttu-id="8ff54-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8ff54-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8ff54-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff54-144">Request</span></span>
<span data-ttu-id="8ff54-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff54-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="8ff54-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff54-146">Response</span></span>
<span data-ttu-id="8ff54-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
