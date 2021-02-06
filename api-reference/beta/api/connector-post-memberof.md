---
title: Adicionar Conector ao connectorGroup
description: Use essa API para adicionar um conector a um novo connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d4d9b9b31eafa0906b704b7f1ff1929b1cf35055
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129598"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="8a4d8-103">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8a4d8-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="8a4d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a4d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a4d8-105">Adicione um [conector](../resources/connector.md)  a um [connectorGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="8a4d8-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8a4d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a4d8-106">Permissions</span></span>
<span data-ttu-id="8a4d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a4d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a4d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a4d8-109">Permission type</span></span>      | <span data-ttu-id="8a4d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a4d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a4d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a4d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4d8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a4d8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a4d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a4d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-114">Not supported.</span></span>    |
|<span data-ttu-id="8a4d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a4d8-115">Application</span></span> | <span data-ttu-id="8a4d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8a4d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a4d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="8a4d8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a4d8-118">Request headers</span></span>
| <span data-ttu-id="8a4d8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8a4d8-119">Name</span></span>       | <span data-ttu-id="8a4d8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a4d8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a4d8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a4d8-121">Authorization</span></span>  | <span data-ttu-id="8a4d8-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-122">Bearer.</span></span> <span data-ttu-id="8a4d8-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a4d8-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a4d8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a4d8-124">Request body</span></span>
<span data-ttu-id="8a4d8-125">No corpo da solicitação, fornece uma representação JSON do [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8a4d8-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8a4d8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a4d8-126">Response</span></span>

<span data-ttu-id="8a4d8-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a4d8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a4d8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a4d8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a4d8-129">Request</span></span>
<span data-ttu-id="8a4d8-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a4d8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a4d8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="8a4d8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a4d8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8a4d8-133">C#</span><span class="sxs-lookup"><span data-stu-id="8a4d8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a4d8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a4d8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a4d8-135">Java</span><span class="sxs-lookup"><span data-stu-id="8a4d8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8a4d8-136">No corpo da solicitação, fornece uma representação JSON do [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8a4d8-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8a4d8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a4d8-137">Response</span></span>
<span data-ttu-id="8a4d8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a4d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



