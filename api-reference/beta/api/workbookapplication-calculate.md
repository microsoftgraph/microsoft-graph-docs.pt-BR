---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fae86c0a8c1511abb1780e03b36ed4edcc329e1b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348337"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="a4c17-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="a4c17-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4c17-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="a4c17-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4c17-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4c17-105">Permissions</span></span>
<span data-ttu-id="a4c17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4c17-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c17-108">Permission type</span></span>      | <span data-ttu-id="a4c17-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4c17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4c17-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4c17-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c17-111">Not supported.</span></span>    |
|<span data-ttu-id="a4c17-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4c17-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c17-113">Not supported.</span></span>    |
|<span data-ttu-id="a4c17-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c17-114">Application</span></span> | <span data-ttu-id="a4c17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4c17-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c17-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="a4c17-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c17-117">Request headers</span></span>
| <span data-ttu-id="a4c17-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a4c17-118">Name</span></span>       | <span data-ttu-id="a4c17-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4c17-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4c17-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4c17-120">Authorization</span></span>  | <span data-ttu-id="a4c17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4c17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4c17-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c17-123">Request body</span></span>
<span data-ttu-id="a4c17-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4c17-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4c17-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4c17-125">Parameter</span></span>    | <span data-ttu-id="a4c17-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4c17-126">Type</span></span>   |<span data-ttu-id="a4c17-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4c17-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4c17-128">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="a4c17-128">calculationType</span></span>|<span data-ttu-id="a4c17-129">string</span><span class="sxs-lookup"><span data-stu-id="a4c17-129">string</span></span>|<span data-ttu-id="a4c17-130">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="a4c17-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="a4c17-131">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="a4c17-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="a4c17-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c17-132">Response</span></span>

<span data-ttu-id="a4c17-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c17-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4c17-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4c17-135">Example</span></span>
<span data-ttu-id="a4c17-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a4c17-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4c17-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c17-137">Request</span></span>
<span data-ttu-id="a4c17-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4c17-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="a4c17-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c17-139">Response</span></span>
<span data-ttu-id="a4c17-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c17-140">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
