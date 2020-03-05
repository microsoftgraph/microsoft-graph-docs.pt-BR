---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dce30f90f35bb373be845aaa9390c9da8c54d02f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437179"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="59ebc-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="59ebc-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="59ebc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59ebc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59ebc-105">Use esta API para adicionar um conector a um conector.</span><span class="sxs-lookup"><span data-stu-id="59ebc-105">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="59ebc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59ebc-106">Permissions</span></span>
<span data-ttu-id="59ebc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59ebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59ebc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59ebc-109">Permission type</span></span>      | <span data-ttu-id="59ebc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59ebc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59ebc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59ebc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59ebc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59ebc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59ebc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59ebc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59ebc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59ebc-114">Not supported.</span></span>    |
|<span data-ttu-id="59ebc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59ebc-115">Application</span></span> | <span data-ttu-id="59ebc-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ebc-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59ebc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59ebc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="59ebc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59ebc-118">Request headers</span></span>
| <span data-ttu-id="59ebc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="59ebc-119">Name</span></span>       | <span data-ttu-id="59ebc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="59ebc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59ebc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59ebc-121">Authorization</span></span>  | <span data-ttu-id="59ebc-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="59ebc-122">Bearer.</span></span> <span data-ttu-id="59ebc-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="59ebc-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="59ebc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59ebc-124">Request body</span></span>
<span data-ttu-id="59ebc-125">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="59ebc-125">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59ebc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="59ebc-126">Response</span></span>

<span data-ttu-id="59ebc-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59ebc-127">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59ebc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59ebc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59ebc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59ebc-129">Request</span></span>
<span data-ttu-id="59ebc-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59ebc-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connector/{id}"
}
```
<span data-ttu-id="59ebc-131">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="59ebc-131">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="59ebc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="59ebc-132">Response</span></span>
<span data-ttu-id="59ebc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59ebc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
