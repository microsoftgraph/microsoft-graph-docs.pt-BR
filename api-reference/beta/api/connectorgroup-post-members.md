---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b147b384223bee7bc7eb245b11e19c5600d0fed
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681177"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="7d199-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="7d199-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="7d199-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d199-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d199-105">Adicionar um [conector](../resources/connector.md) a um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="7d199-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="7d199-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d199-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d199-108">Permission type</span></span>      | <span data-ttu-id="7d199-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d199-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d199-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d199-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d199-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d199-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d199-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d199-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d199-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d199-113">Not supported.</span></span>    |
|<span data-ttu-id="7d199-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d199-114">Application</span></span> | <span data-ttu-id="7d199-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d199-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7d199-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d199-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7d199-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d199-117">Request headers</span></span>
| <span data-ttu-id="7d199-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7d199-118">Name</span></span>       | <span data-ttu-id="7d199-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d199-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d199-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d199-120">Authorization</span></span>  | <span data-ttu-id="7d199-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="7d199-121">Bearer.</span></span> <span data-ttu-id="7d199-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7d199-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d199-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d199-123">Request body</span></span>
<span data-ttu-id="7d199-124">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="7d199-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7d199-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d199-125">Response</span></span>

<span data-ttu-id="7d199-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d199-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d199-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d199-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d199-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d199-128">Request</span></span>
<span data-ttu-id="7d199-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d199-129">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d199-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d199-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="7d199-131">C#</span><span class="sxs-lookup"><span data-stu-id="7d199-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d199-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d199-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d199-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d199-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7d199-134">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="7d199-134">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7d199-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d199-135">Response</span></span>
<span data-ttu-id="7d199-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d199-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
