---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad5efa59698d4dcf05365c63eb7f69fa2eb095a6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862924"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="e0adb-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="e0adb-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="e0adb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0adb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0adb-105">Adicionar um [conector](../resources/connector.md) a um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e0adb-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="e0adb-106">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e0adb-106">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e0adb-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0adb-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0adb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0adb-108">Permission type</span></span>      | <span data-ttu-id="e0adb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0adb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0adb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0adb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0adb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0adb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0adb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0adb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0adb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0adb-113">Not supported.</span></span>    |
|<span data-ttu-id="e0adb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0adb-114">Application</span></span> | <span data-ttu-id="e0adb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0adb-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e0adb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0adb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="e0adb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0adb-117">Request headers</span></span>
| <span data-ttu-id="e0adb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e0adb-118">Name</span></span>       | <span data-ttu-id="e0adb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0adb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0adb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0adb-120">Authorization</span></span>  | <span data-ttu-id="e0adb-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="e0adb-121">Bearer.</span></span> <span data-ttu-id="e0adb-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0adb-122">Required.</span></span>|
| <span data-ttu-id="e0adb-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="e0adb-123">Content-type</span></span> | <span data-ttu-id="e0adb-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="e0adb-124">application/json.</span></span> <span data-ttu-id="e0adb-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e0adb-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0adb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0adb-126">Request body</span></span>
<span data-ttu-id="e0adb-127">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="e0adb-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0adb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0adb-128">Response</span></span>

<span data-ttu-id="e0adb-129">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0adb-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0adb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0adb-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0adb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0adb-131">Request</span></span>
<span data-ttu-id="e0adb-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0adb-132">The following is an example of the request.</span></span>
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
### <a name="response"></a><span data-ttu-id="e0adb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0adb-133">Response</span></span>
<span data-ttu-id="e0adb-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0adb-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add connector to connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
