---
title: Obtenha o aplicativo
description: Recupere as propriedades e relações do objeto application.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 833a6470a1db8cef0ce26ca4cecfe1c5039fa159
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935826"
---
# <a name="get-application"></a><span data-ttu-id="b7bdf-103">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7bdf-103">Get Application</span></span>

> <span data-ttu-id="b7bdf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7bdf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7bdf-106">Recupere as propriedades e relações do objeto application.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-106">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7bdf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7bdf-107">Permissions</span></span>
<span data-ttu-id="b7bdf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7bdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7bdf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7bdf-110">Permission type</span></span>      | <span data-ttu-id="b7bdf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7bdf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7bdf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7bdf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7bdf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-113">Not supported.</span></span>    |
|<span data-ttu-id="b7bdf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7bdf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7bdf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-115">Not supported.</span></span>    |
|<span data-ttu-id="b7bdf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7bdf-116">Application</span></span> | <span data-ttu-id="b7bdf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7bdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7bdf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7bdf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7bdf-119">Optional query parameters</span></span>
<span data-ttu-id="b7bdf-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7bdf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bdf-121">Request headers</span></span>
| <span data-ttu-id="b7bdf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b7bdf-122">Name</span></span>      |<span data-ttu-id="b7bdf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7bdf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7bdf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7bdf-124">Authorization</span></span>  | <span data-ttu-id="b7bdf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7bdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bdf-127">Request body</span></span>
<span data-ttu-id="b7bdf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7bdf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7bdf-129">Response</span></span>

<span data-ttu-id="b7bdf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [aplicativo](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-130">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7bdf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7bdf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7bdf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bdf-132">Request</span></span>
<span data-ttu-id="b7bdf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="b7bdf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7bdf-134">Response</span></span>
<span data-ttu-id="b7bdf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7bdf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
