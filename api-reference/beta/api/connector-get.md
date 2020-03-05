---
title: Obter conector
description: Recupere as propriedades de um objeto Connector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b8e8fc8bc23726c31244c989dc2821e56bb36908
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437788"
---
# <a name="get-connector"></a><span data-ttu-id="d1ffc-103">Obter conector</span><span class="sxs-lookup"><span data-stu-id="d1ffc-103">Get connector</span></span>

<span data-ttu-id="d1ffc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1ffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1ffc-105">Recupere as propriedades de um objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-105">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1ffc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1ffc-106">Permissions</span></span>
<span data-ttu-id="d1ffc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ffc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1ffc-109">Permission type</span></span>      | <span data-ttu-id="d1ffc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1ffc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1ffc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1ffc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1ffc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1ffc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1ffc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1ffc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1ffc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-114">Not supported.</span></span>    |
|<span data-ttu-id="d1ffc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1ffc-115">Application</span></span> | <span data-ttu-id="d1ffc-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ffc-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1ffc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1ffc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1ffc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1ffc-118">Optional query parameters</span></span>
<span data-ttu-id="d1ffc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ffc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1ffc-120">Request headers</span></span>
| <span data-ttu-id="d1ffc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d1ffc-121">Name</span></span>      |<span data-ttu-id="d1ffc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ffc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1ffc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1ffc-123">Authorization</span></span>  | <span data-ttu-id="d1ffc-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-124">Bearer.</span></span> <span data-ttu-id="d1ffc-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="d1ffc-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1ffc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1ffc-126">Request body</span></span>
<span data-ttu-id="d1ffc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1ffc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1ffc-128">Response</span></span>

<span data-ttu-id="d1ffc-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1ffc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1ffc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1ffc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1ffc-131">Request</span></span>
<span data-ttu-id="d1ffc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="d1ffc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1ffc-133">Response</span></span>
<span data-ttu-id="d1ffc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1ffc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
