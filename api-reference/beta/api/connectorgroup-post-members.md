---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c8b428ca6c724ce37116430cbae56587866c13eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943383"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="53890-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="53890-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53890-104">Use esta API para adicionar um conector a um conector.</span><span class="sxs-lookup"><span data-stu-id="53890-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="53890-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="53890-105">Permissions</span></span>
<span data-ttu-id="53890-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53890-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53890-108">Permission type</span></span>      | <span data-ttu-id="53890-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53890-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53890-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53890-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53890-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53890-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53890-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53890-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53890-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53890-113">Not supported.</span></span>    |
|<span data-ttu-id="53890-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53890-114">Application</span></span> | <span data-ttu-id="53890-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53890-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53890-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53890-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="53890-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53890-117">Request headers</span></span>
| <span data-ttu-id="53890-118">Nome</span><span class="sxs-lookup"><span data-stu-id="53890-118">Name</span></span>       | <span data-ttu-id="53890-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="53890-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53890-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="53890-120">Authorization</span></span>  | <span data-ttu-id="53890-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="53890-121">Bearer.</span></span> <span data-ttu-id="53890-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="53890-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="53890-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53890-123">Request body</span></span>
<span data-ttu-id="53890-124">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="53890-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53890-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="53890-125">Response</span></span>

<span data-ttu-id="53890-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53890-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53890-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53890-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53890-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53890-128">Request</span></span>
<span data-ttu-id="53890-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53890-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="53890-130">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="53890-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="53890-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="53890-131">Response</span></span>
<span data-ttu-id="53890-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53890-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
