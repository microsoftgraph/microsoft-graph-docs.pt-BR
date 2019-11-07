---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos de um objeto workbookApplication.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f265fe51ce37504b331ee735f9d3fa91979f5891
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023231"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="0d60a-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="0d60a-103">Get workbookApplication</span></span>

<span data-ttu-id="0d60a-104">Recupere as propriedades e os relacionamentos de um objeto [workbookApplication](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="0d60a-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d60a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d60a-105">Permissions</span></span>
<span data-ttu-id="0d60a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d60a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d60a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d60a-108">Permission type</span></span>      | <span data-ttu-id="0d60a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d60a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d60a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d60a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d60a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d60a-111">Files.ReadWrite</span></span>   |
|<span data-ttu-id="0d60a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d60a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d60a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d60a-113">Not supported.</span></span>    |
|<span data-ttu-id="0d60a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d60a-114">Application</span></span> | <span data-ttu-id="0d60a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d60a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d60a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d60a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="0d60a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d60a-117">Request headers</span></span>
| <span data-ttu-id="0d60a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0d60a-118">Name</span></span>      |<span data-ttu-id="0d60a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d60a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d60a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d60a-120">Authorization</span></span>  | <span data-ttu-id="0d60a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d60a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d60a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d60a-123">Request body</span></span>
<span data-ttu-id="0d60a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d60a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d60a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d60a-125">Response</span></span>

<span data-ttu-id="0d60a-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d60a-126">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d60a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d60a-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d60a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d60a-128">Request</span></span>
<span data-ttu-id="0d60a-129">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d60a-129">Here is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```

### <a name="response"></a><span data-ttu-id="0d60a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d60a-130">Response</span></span>
<span data-ttu-id="0d60a-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d60a-131">Here is an example of the response.</span></span> 

> <span data-ttu-id="0d60a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d60a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
