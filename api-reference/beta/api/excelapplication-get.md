---
title: Obtenha o aplicativo
description: Recupere as propriedades e relações do objeto application.
localization_priority: Normal
ms.openlocfilehash: 9226e697f3e8439740003887d8560ffaac9df2fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864488"
---
# <a name="get-application"></a><span data-ttu-id="8aaf8-103">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aaf8-103">Get Application</span></span>

> <span data-ttu-id="8aaf8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8aaf8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8aaf8-106">Recupere as propriedades e relações do objeto application.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-106">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8aaf8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8aaf8-107">Permissions</span></span>
<span data-ttu-id="8aaf8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aaf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aaf8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aaf8-110">Permission type</span></span>      | <span data-ttu-id="8aaf8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8aaf8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aaf8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aaf8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8aaf8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-113">Not supported.</span></span>    |
|<span data-ttu-id="8aaf8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aaf8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aaf8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-115">Not supported.</span></span>    |
|<span data-ttu-id="8aaf8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aaf8-116">Application</span></span> | <span data-ttu-id="8aaf8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aaf8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aaf8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8aaf8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8aaf8-119">Optional query parameters</span></span>
<span data-ttu-id="8aaf8-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aaf8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aaf8-121">Request headers</span></span>
| <span data-ttu-id="8aaf8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8aaf8-122">Name</span></span>      |<span data-ttu-id="8aaf8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aaf8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8aaf8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aaf8-124">Authorization</span></span>  | <span data-ttu-id="8aaf8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aaf8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aaf8-127">Request body</span></span>
<span data-ttu-id="8aaf8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aaf8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aaf8-129">Response</span></span>

<span data-ttu-id="8aaf8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [aplicativo](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-130">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8aaf8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aaf8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8aaf8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aaf8-132">Request</span></span>
<span data-ttu-id="8aaf8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="8aaf8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aaf8-134">Response</span></span>
<span data-ttu-id="8aaf8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aaf8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
