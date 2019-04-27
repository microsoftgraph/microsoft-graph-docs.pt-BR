---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 75acf7e2abeb44bc332d64056a9815369163f423
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348340"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="2a54f-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="2a54f-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a54f-104">Recupere as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="2a54f-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a54f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a54f-105">Permissions</span></span>
<span data-ttu-id="2a54f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a54f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a54f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a54f-108">Permission type</span></span>      | <span data-ttu-id="2a54f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a54f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a54f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a54f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a54f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a54f-111">Not supported.</span></span>    |
|<span data-ttu-id="2a54f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a54f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a54f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a54f-113">Not supported.</span></span>    |
|<span data-ttu-id="2a54f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a54f-114">Application</span></span> | <span data-ttu-id="2a54f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a54f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a54f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a54f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a54f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a54f-117">Optional query parameters</span></span>
<span data-ttu-id="2a54f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a54f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a54f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a54f-119">Request headers</span></span>
| <span data-ttu-id="2a54f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2a54f-120">Name</span></span>      |<span data-ttu-id="2a54f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a54f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a54f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a54f-122">Authorization</span></span>  | <span data-ttu-id="2a54f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a54f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a54f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a54f-125">Request body</span></span>
<span data-ttu-id="2a54f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a54f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a54f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a54f-127">Response</span></span>

<span data-ttu-id="2a54f-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a54f-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a54f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a54f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a54f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a54f-130">Request</span></span>
<span data-ttu-id="2a54f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a54f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="2a54f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a54f-132">Response</span></span>
<span data-ttu-id="2a54f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a54f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
