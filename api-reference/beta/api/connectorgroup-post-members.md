---
title: Adicionar um conector para connectorGroup
description: Use essa API para adicionar um conector a um connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 8df6fdda80007217164f8ae2f21a1d3f8d667d23
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518251"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="e2370-103">Adicionar um conector para connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e2370-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2370-104">Use essa API para adicionar um conector a um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="e2370-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2370-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2370-105">Permissions</span></span>
<span data-ttu-id="e2370-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2370-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2370-108">Permission type</span></span>      | <span data-ttu-id="e2370-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2370-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2370-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2370-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2370-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2370-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2370-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2370-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2370-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2370-113">Not supported.</span></span>    |
|<span data-ttu-id="e2370-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2370-114">Application</span></span> | <span data-ttu-id="e2370-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2370-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2370-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2370-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e2370-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2370-117">Request headers</span></span>
| <span data-ttu-id="e2370-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e2370-118">Name</span></span>       | <span data-ttu-id="e2370-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2370-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2370-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2370-120">Authorization</span></span>  | <span data-ttu-id="e2370-121"> de portador</span><span class="sxs-lookup"><span data-stu-id="e2370-121">Bearer.</span></span> <span data-ttu-id="e2370-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e2370-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2370-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2370-123">Request body</span></span>
<span data-ttu-id="e2370-124">No corpo da solicitação, fornece uma representação JSON de um link para um objeto de [conector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="e2370-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2370-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2370-125">Response</span></span>

<span data-ttu-id="e2370-126">Se tiver êxito, este método retornará `201 Created` objeto de [conector](../resources/connector.md) e o código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2370-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2370-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2370-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2370-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2370-128">Request</span></span>
<span data-ttu-id="e2370-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2370-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="e2370-130">No corpo da solicitação, fornece uma representação JSON de um link para um objeto de [conector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="e2370-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e2370-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2370-131">Response</span></span>
<span data-ttu-id="e2370-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2370-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
