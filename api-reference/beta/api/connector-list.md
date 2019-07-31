---
title: Conectores de lista
description: Recupere uma lista de objetos Connector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a85a1d478adc37da6dafe7850262539993e15ae8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943502"
---
# <a name="list-connectors"></a><span data-ttu-id="406dd-103">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="406dd-103">List connectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="406dd-104">Recupere uma lista de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="406dd-104">Retrieve a list of connector objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="406dd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="406dd-105">Permissions</span></span>
<span data-ttu-id="406dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="406dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="406dd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="406dd-108">Permission type</span></span>      | <span data-ttu-id="406dd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="406dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="406dd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="406dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="406dd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="406dd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="406dd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="406dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="406dd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="406dd-113">Not supported.</span></span>    |
|<span data-ttu-id="406dd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="406dd-114">Application</span></span> | <span data-ttu-id="406dd-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="406dd-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="406dd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="406dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="406dd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="406dd-117">Optional query parameters</span></span>
<span data-ttu-id="406dd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="406dd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="406dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="406dd-119">Request headers</span></span>
| <span data-ttu-id="406dd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="406dd-120">Name</span></span>      |<span data-ttu-id="406dd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="406dd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="406dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="406dd-122">Authorization</span></span>  | <span data-ttu-id="406dd-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="406dd-123">Bearer.</span></span> <span data-ttu-id="406dd-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="406dd-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="406dd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="406dd-125">Request body</span></span>
<span data-ttu-id="406dd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="406dd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="406dd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="406dd-127">Response</span></span>

<span data-ttu-id="406dd-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="406dd-128">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="406dd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="406dd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="406dd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="406dd-130">Request</span></span>
<span data-ttu-id="406dd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="406dd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors
```
##### <a name="response"></a><span data-ttu-id="406dd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="406dd-132">Response</span></span>
<span data-ttu-id="406dd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="406dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
