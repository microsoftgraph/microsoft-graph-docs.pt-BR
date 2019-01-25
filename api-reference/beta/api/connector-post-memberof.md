---
title: Adicionar um conector para connectorGroup
description: Use essa API para adicionar um conector para um novo connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 097f24233ec1c540885d67b60a4b471ff1c64f65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514625"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="22c99-103">Adicionar um conector para connectorGroup</span><span class="sxs-lookup"><span data-stu-id="22c99-103">Add Connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22c99-104">Use essa API para adicionar um conector para um novo connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="22c99-104">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="22c99-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="22c99-105">Permissions</span></span>
<span data-ttu-id="22c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c99-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22c99-108">Permission type</span></span>      | <span data-ttu-id="22c99-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22c99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22c99-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22c99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="22c99-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22c99-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22c99-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22c99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22c99-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22c99-113">Not supported.</span></span>    |
|<span data-ttu-id="22c99-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22c99-114">Application</span></span> | <span data-ttu-id="22c99-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22c99-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22c99-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22c99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="22c99-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22c99-117">Request headers</span></span>
| <span data-ttu-id="22c99-118">Nome</span><span class="sxs-lookup"><span data-stu-id="22c99-118">Name</span></span>       | <span data-ttu-id="22c99-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="22c99-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22c99-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="22c99-120">Authorization</span></span>  | <span data-ttu-id="22c99-121"> de portador</span><span class="sxs-lookup"><span data-stu-id="22c99-121">Bearer.</span></span> <span data-ttu-id="22c99-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="22c99-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="22c99-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22c99-123">Request body</span></span>
<span data-ttu-id="22c99-124">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="22c99-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22c99-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="22c99-125">Response</span></span>

<span data-ttu-id="22c99-126">Se tiver êxito, este método retornará `201 Created` objeto response de código e [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22c99-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22c99-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22c99-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22c99-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22c99-128">Request</span></span>
<span data-ttu-id="22c99-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22c99-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="22c99-130">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="22c99-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="22c99-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22c99-131">Response</span></span>
<span data-ttu-id="22c99-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22c99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connector-post-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
