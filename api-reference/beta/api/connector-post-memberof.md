---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um novo conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d7a6c29674495b960ad9f412b8962e1a66de6244
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719950"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="365e5-103">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="365e5-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="365e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="365e5-105">Adicionar um [conector](../resources/connector.md)  a um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="365e5-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="365e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="365e5-106">Permissions</span></span>
<span data-ttu-id="365e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="365e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="365e5-109">Permission type</span></span>      | <span data-ttu-id="365e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="365e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="365e5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="365e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="365e5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="365e5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="365e5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="365e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="365e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="365e5-114">Not supported.</span></span>    |
|<span data-ttu-id="365e5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="365e5-115">Application</span></span> | <span data-ttu-id="365e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="365e5-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="365e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="365e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="365e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="365e5-118">Request headers</span></span>
| <span data-ttu-id="365e5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="365e5-119">Name</span></span>       | <span data-ttu-id="365e5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="365e5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="365e5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="365e5-121">Authorization</span></span>  | <span data-ttu-id="365e5-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="365e5-122">Bearer.</span></span> <span data-ttu-id="365e5-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="365e5-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="365e5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="365e5-124">Request body</span></span>
<span data-ttu-id="365e5-125">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="365e5-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="365e5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="365e5-126">Response</span></span>

<span data-ttu-id="365e5-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="365e5-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="365e5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="365e5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="365e5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="365e5-129">Request</span></span>
<span data-ttu-id="365e5-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="365e5-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="365e5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="365e5-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="365e5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="365e5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="365e5-133">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="365e5-133">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="365e5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="365e5-134">Response</span></span>
<span data-ttu-id="365e5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="365e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


