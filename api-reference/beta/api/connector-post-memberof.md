---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um novo conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 85ea1046509cc0937b9f2ad0d6372dcc1b222862
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943506"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="b2ff6-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="b2ff6-103">Add Connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2ff6-104">Use esta API para adicionar um conector a um novo conector.</span><span class="sxs-lookup"><span data-stu-id="b2ff6-104">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2ff6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2ff6-105">Permissions</span></span>
<span data-ttu-id="b2ff6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2ff6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2ff6-108">Permission type</span></span>      | <span data-ttu-id="b2ff6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2ff6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2ff6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2ff6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2ff6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2ff6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2ff6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2ff6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2ff6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2ff6-113">Not supported.</span></span>    |
|<span data-ttu-id="b2ff6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2ff6-114">Application</span></span> | <span data-ttu-id="b2ff6-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2ff6-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2ff6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2ff6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="b2ff6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2ff6-117">Request headers</span></span>
| <span data-ttu-id="b2ff6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b2ff6-118">Name</span></span>       | <span data-ttu-id="b2ff6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2ff6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2ff6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2ff6-120">Authorization</span></span>  | <span data-ttu-id="b2ff6-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="b2ff6-121">Bearer.</span></span> <span data-ttu-id="b2ff6-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b2ff6-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2ff6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2ff6-123">Request body</span></span>
<span data-ttu-id="b2ff6-124">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b2ff6-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b2ff6-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2ff6-125">Response</span></span>

<span data-ttu-id="b2ff6-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto de teleconnector no corpo da resposta. [](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b2ff6-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2ff6-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2ff6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2ff6-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2ff6-128">Request</span></span>
<span data-ttu-id="b2ff6-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2ff6-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connectorGroups/{id}"
}
```
<span data-ttu-id="b2ff6-130">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b2ff6-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b2ff6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2ff6-131">Response</span></span>
<span data-ttu-id="b2ff6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2ff6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isDefault": false
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
