---
title: 'Aplicativo: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f16c858f7e8c9d85dbe8252bde0a791bc325514c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463999"
---
# <a name="application-calculate"></a><span data-ttu-id="77a9b-103">Aplicativo: calcular</span><span class="sxs-lookup"><span data-stu-id="77a9b-103">Application: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77a9b-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="77a9b-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="77a9b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="77a9b-105">Permissions</span></span>
<span data-ttu-id="77a9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a9b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77a9b-108">Permission type</span></span>      | <span data-ttu-id="77a9b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77a9b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77a9b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77a9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77a9b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77a9b-111">Not supported.</span></span>    |
|<span data-ttu-id="77a9b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77a9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a9b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77a9b-113">Not supported.</span></span>    |
|<span data-ttu-id="77a9b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77a9b-114">Application</span></span> | <span data-ttu-id="77a9b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77a9b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77a9b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77a9b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="77a9b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77a9b-117">Request headers</span></span>
| <span data-ttu-id="77a9b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="77a9b-118">Name</span></span>       | <span data-ttu-id="77a9b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="77a9b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77a9b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="77a9b-120">Authorization</span></span>  | <span data-ttu-id="77a9b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77a9b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77a9b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77a9b-123">Request body</span></span>
<span data-ttu-id="77a9b-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77a9b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77a9b-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77a9b-125">Parameter</span></span>    | <span data-ttu-id="77a9b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="77a9b-126">Type</span></span>   |<span data-ttu-id="77a9b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="77a9b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a9b-128">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="77a9b-128">calculationType</span></span>|<span data-ttu-id="77a9b-129">string</span><span class="sxs-lookup"><span data-stu-id="77a9b-129">string</span></span>|<span data-ttu-id="77a9b-130">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="77a9b-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="77a9b-131">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="77a9b-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="77a9b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="77a9b-132">Response</span></span>

<span data-ttu-id="77a9b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77a9b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77a9b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77a9b-135">Example</span></span>
<span data-ttu-id="77a9b-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="77a9b-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="77a9b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77a9b-137">Request</span></span>
<span data-ttu-id="77a9b-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77a9b-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="77a9b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77a9b-139">Response</span></span>
<span data-ttu-id="77a9b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77a9b-140">Here is an example of the response.</span></span> 
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
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/excelapplication-calculate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
