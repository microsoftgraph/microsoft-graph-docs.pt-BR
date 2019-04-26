---
title: Adicionar conector ao conector
description: Use esta API para adicionar um conector a um conector.
localization_priority: Normal
ms.openlocfilehash: 839189b323318b440608b699864a36b69a6c840d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327595"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="8b709-103">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="8b709-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b709-104">Use esta API para adicionar um conector a um conector.</span><span class="sxs-lookup"><span data-stu-id="8b709-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b709-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b709-105">Permissions</span></span>
<span data-ttu-id="8b709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b709-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b709-108">Permission type</span></span>      | <span data-ttu-id="8b709-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b709-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b709-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b709-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b709-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b709-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b709-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b709-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b709-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b709-113">Not supported.</span></span>    |
|<span data-ttu-id="8b709-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b709-114">Application</span></span> | <span data-ttu-id="8b709-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b709-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b709-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b709-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8b709-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b709-117">Request headers</span></span>
| <span data-ttu-id="8b709-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8b709-118">Name</span></span>       | <span data-ttu-id="8b709-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b709-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b709-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b709-120">Authorization</span></span>  | <span data-ttu-id="8b709-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="8b709-121">Bearer.</span></span> <span data-ttu-id="8b709-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b709-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b709-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b709-123">Request body</span></span>
<span data-ttu-id="8b709-124">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="8b709-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b709-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b709-125">Response</span></span>

<span data-ttu-id="8b709-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b709-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b709-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b709-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b709-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b709-128">Request</span></span>
<span data-ttu-id="8b709-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b709-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="8b709-130">No corpo da solicitação, forneça uma representação JSON de um link para um objeto [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="8b709-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8b709-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b709-131">Response</span></span>
<span data-ttu-id="8b709-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b709-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
