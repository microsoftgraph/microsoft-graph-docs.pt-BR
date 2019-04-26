---
title: 'TableCollection: add'
description: Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ba339cd0d3be6c46d9280b19e774f2a0062f616b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335539"
---
# <a name="tablecollection-add"></a><span data-ttu-id="dd459-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="dd459-105">TableCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd459-p102">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="dd459-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="dd459-109">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="dd459-109">Error Handling</span></span>

<span data-ttu-id="dd459-110">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="dd459-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="dd459-111">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd459-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd459-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd459-112">Permissions</span></span>
<span data-ttu-id="dd459-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd459-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd459-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd459-115">Permission type</span></span>      | <span data-ttu-id="dd459-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd459-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd459-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd459-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dd459-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd459-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd459-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd459-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd459-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd459-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd459-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd459-121">Application</span></span> | <span data-ttu-id="dd459-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd459-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd459-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd459-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="dd459-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd459-124">Request headers</span></span>
| <span data-ttu-id="dd459-125">Nome</span><span class="sxs-lookup"><span data-stu-id="dd459-125">Name</span></span>       | <span data-ttu-id="dd459-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd459-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd459-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd459-127">Authorization</span></span>  | <span data-ttu-id="dd459-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd459-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd459-130">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd459-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd459-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd459-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd459-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd459-133">Request body</span></span>
<span data-ttu-id="dd459-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd459-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd459-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dd459-135">Parameter</span></span>    | <span data-ttu-id="dd459-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd459-136">Type</span></span>   |<span data-ttu-id="dd459-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd459-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd459-138">address</span><span class="sxs-lookup"><span data-stu-id="dd459-138">address</span></span>|<span data-ttu-id="dd459-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd459-139">string</span></span>|<span data-ttu-id="dd459-p107">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="dd459-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="dd459-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="dd459-142">hasHeaders</span></span>|<span data-ttu-id="dd459-143">booliano</span><span class="sxs-lookup"><span data-stu-id="dd459-143">boolean</span></span>|<span data-ttu-id="dd459-p108">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="dd459-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="dd459-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd459-147">Response</span></span>

<span data-ttu-id="dd459-148">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbooktable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd459-148">If successful, this method returns `200 OK` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd459-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd459-149">Example</span></span>
<span data-ttu-id="dd459-150">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dd459-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd459-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd459-151">Request</span></span>
<span data-ttu-id="dd459-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd459-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="dd459-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd459-153">Response</span></span>
<span data-ttu-id="dd459-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd459-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
