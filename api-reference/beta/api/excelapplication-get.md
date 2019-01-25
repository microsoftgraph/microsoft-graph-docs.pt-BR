---
title: Obtenha o aplicativo
description: Recupere as propriedades e relações do objeto application.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 024e2cde999e90b1f361e7f67ca28ddd71078824
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522921"
---
# <a name="get-application"></a><span data-ttu-id="ec7c3-103">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec7c3-103">Get Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec7c3-104">Recupere as propriedades e relações do objeto application.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-104">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec7c3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec7c3-105">Permissions</span></span>
<span data-ttu-id="ec7c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec7c3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec7c3-108">Permission type</span></span>      | <span data-ttu-id="ec7c3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec7c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec7c3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec7c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec7c3-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-111">Not supported.</span></span>    |
|<span data-ttu-id="ec7c3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec7c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec7c3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-113">Not supported.</span></span>    |
|<span data-ttu-id="ec7c3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec7c3-114">Application</span></span> | <span data-ttu-id="ec7c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec7c3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec7c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec7c3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec7c3-117">Optional query parameters</span></span>
<span data-ttu-id="ec7c3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec7c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7c3-119">Request headers</span></span>
| <span data-ttu-id="ec7c3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ec7c3-120">Name</span></span>      |<span data-ttu-id="ec7c3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec7c3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec7c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec7c3-122">Authorization</span></span>  | <span data-ttu-id="ec7c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec7c3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7c3-125">Request body</span></span>
<span data-ttu-id="ec7c3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec7c3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec7c3-127">Response</span></span>

<span data-ttu-id="ec7c3-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [aplicativo](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-128">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec7c3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec7c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec7c3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7c3-130">Request</span></span>
<span data-ttu-id="ec7c3-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="ec7c3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec7c3-132">Response</span></span>
<span data-ttu-id="ec7c3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec7c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
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
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/excelapplication-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
