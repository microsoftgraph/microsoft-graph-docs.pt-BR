---
title: 'TableCollection: add'
description: Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.
ms.openlocfilehash: 6435abe4a2671ec3937b7f1b0bbda8825fad1c7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039834"
---
# <a name="tablecollection-add"></a><span data-ttu-id="07600-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="07600-105">TableCollection: add</span></span>

> <span data-ttu-id="07600-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07600-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07600-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07600-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07600-p103">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="07600-p103">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="07600-111">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="07600-111">Error Handling</span></span>

<span data-ttu-id="07600-112">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="07600-112">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="07600-113">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="07600-113">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="07600-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="07600-114">Permissions</span></span>
<span data-ttu-id="07600-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07600-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07600-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07600-117">Permission type</span></span>      | <span data-ttu-id="07600-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07600-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07600-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07600-119">Delegated (work or school account)</span></span> | <span data-ttu-id="07600-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07600-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07600-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07600-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07600-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07600-122">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07600-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07600-123">Application</span></span> | <span data-ttu-id="07600-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07600-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07600-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07600-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="07600-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07600-126">Request headers</span></span>
| <span data-ttu-id="07600-127">Nome</span><span class="sxs-lookup"><span data-stu-id="07600-127">Name</span></span>       | <span data-ttu-id="07600-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="07600-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07600-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="07600-129">Authorization</span></span>  | <span data-ttu-id="07600-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07600-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07600-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="07600-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="07600-p107">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="07600-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07600-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07600-135">Request body</span></span>
<span data-ttu-id="07600-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07600-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07600-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="07600-137">Parameter</span></span>    | <span data-ttu-id="07600-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="07600-138">Type</span></span>   |<span data-ttu-id="07600-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="07600-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07600-140">address</span><span class="sxs-lookup"><span data-stu-id="07600-140">address</span></span>|<span data-ttu-id="07600-141">string</span><span class="sxs-lookup"><span data-stu-id="07600-141">string</span></span>|<span data-ttu-id="07600-p108">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="07600-p108">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="07600-144">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="07600-144">hasHeaders</span></span>|<span data-ttu-id="07600-145">booliano</span><span class="sxs-lookup"><span data-stu-id="07600-145">boolean</span></span>|<span data-ttu-id="07600-p109">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="07600-p109">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="07600-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="07600-149">Response</span></span>

<span data-ttu-id="07600-150">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07600-150">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07600-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07600-151">Example</span></span>
<span data-ttu-id="07600-152">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="07600-152">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="07600-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07600-153">Request</span></span>
<span data-ttu-id="07600-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07600-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="07600-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="07600-155">Response</span></span>
<span data-ttu-id="07600-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07600-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
