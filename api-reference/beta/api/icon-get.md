---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 409f15875e910998acc7035c7b54436108fd1002
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040866"
---
# <a name="get-icon"></a><span data-ttu-id="7ce46-103">Get Icon</span><span class="sxs-lookup"><span data-stu-id="7ce46-103">Get Icon</span></span>

<span data-ttu-id="7ce46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ce46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ce46-105">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="7ce46-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ce46-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ce46-106">Permissions</span></span>
<span data-ttu-id="7ce46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce46-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ce46-109">Permission type</span></span>      | <span data-ttu-id="7ce46-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ce46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ce46-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ce46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ce46-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce46-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ce46-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ce46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ce46-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce46-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ce46-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ce46-115">Application</span></span> | <span data-ttu-id="7ce46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ce46-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ce46-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ce46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ce46-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ce46-118">Optional query parameters</span></span>
<span data-ttu-id="7ce46-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce46-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ce46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce46-120">Request headers</span></span>
| <span data-ttu-id="7ce46-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7ce46-121">Name</span></span>      |<span data-ttu-id="7ce46-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce46-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ce46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ce46-123">Authorization</span></span>  | <span data-ttu-id="7ce46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ce46-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ce46-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce46-126">Request body</span></span>
<span data-ttu-id="7ce46-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ce46-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ce46-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce46-128">Response</span></span>

<span data-ttu-id="7ce46-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookIcon](../resources/workbookicon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce46-129">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ce46-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ce46-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ce46-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce46-131">Request</span></span>
<span data-ttu-id="7ce46-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ce46-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="7ce46-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce46-133">Response</span></span>
<span data-ttu-id="7ce46-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce46-134">Here is an example of the response.</span></span> <span data-ttu-id="7ce46-135">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ce46-135">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->