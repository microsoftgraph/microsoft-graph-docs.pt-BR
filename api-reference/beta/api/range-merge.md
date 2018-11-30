---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
ms.openlocfilehash: 8680afec198cebb820fc695cf7714494a2539cdc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037069"
---
# <a name="range-merge"></a><span data-ttu-id="1a1d6-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="1a1d6-103">Range: merge</span></span>

> <span data-ttu-id="1a1d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a1d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a1d6-106">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a1d6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a1d6-107">Permissions</span></span>
<span data-ttu-id="1a1d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a1d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a1d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a1d6-110">Permission type</span></span>      | <span data-ttu-id="1a1d6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a1d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a1d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a1d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a1d6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a1d6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a1d6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a1d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a1d6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a1d6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a1d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a1d6-116">Application</span></span> | <span data-ttu-id="1a1d6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a1d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a1d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="1a1d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d6-119">Request headers</span></span>
| <span data-ttu-id="1a1d6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1a1d6-120">Name</span></span>       | <span data-ttu-id="1a1d6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1d6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a1d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a1d6-122">Authorization</span></span>  | <span data-ttu-id="1a1d6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a1d6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1a1d6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a1d6-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a1d6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d6-128">Request body</span></span>
<span data-ttu-id="1a1d6-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a1d6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a1d6-130">Parameter</span></span>    | <span data-ttu-id="1a1d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1d6-131">Type</span></span>   |<span data-ttu-id="1a1d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1d6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1d6-133">across</span><span class="sxs-lookup"><span data-stu-id="1a1d6-133">across</span></span>|<span data-ttu-id="1a1d6-134">booliano</span><span class="sxs-lookup"><span data-stu-id="1a1d6-134">boolean</span></span>|<span data-ttu-id="1a1d6-p105">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="1a1d6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1d6-138">Response</span></span>

<span data-ttu-id="1a1d6-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1d6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a1d6-141">Example</span></span>
<span data-ttu-id="1a1d6-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a1d6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d6-143">Request</span></span>
<span data-ttu-id="1a1d6-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="1a1d6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1d6-145">Response</span></span>
<span data-ttu-id="1a1d6-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1d6-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->