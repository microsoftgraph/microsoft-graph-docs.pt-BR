---
title: Criar um conector
description: Use esta API para criar um novo conector.
localization_priority: Normal
ms.openlocfilehash: 90b3d0cdbdd02876e1dfaf3d6743f6dac2199202
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327594"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="5c7a5-103">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="5c7a5-103">Create connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c7a5-104">Use esta API para criar um novo conector.</span><span class="sxs-lookup"><span data-stu-id="5c7a5-104">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c7a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c7a5-105">Permissions</span></span>
<span data-ttu-id="5c7a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c7a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c7a5-108">Permission type</span></span>      | <span data-ttu-id="5c7a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c7a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c7a5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c7a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c7a5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c7a5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c7a5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c7a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c7a5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c7a5-113">Not supported.</span></span>    |
|<span data-ttu-id="5c7a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c7a5-114">Application</span></span> | <span data-ttu-id="5c7a5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c7a5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c7a5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c7a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="5c7a5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7a5-117">Request headers</span></span>
| <span data-ttu-id="5c7a5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5c7a5-118">Name</span></span>       | <span data-ttu-id="5c7a5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7a5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c7a5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c7a5-120">Authorization</span></span>  | <span data-ttu-id="5c7a5-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="5c7a5-121">Bearer.</span></span> <span data-ttu-id="5c7a5-122">Requried</span><span class="sxs-lookup"><span data-stu-id="5c7a5-122">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c7a5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7a5-123">Request body</span></span>
<span data-ttu-id="5c7a5-124">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5c7a5-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5c7a5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c7a5-125">Response</span></span>

<span data-ttu-id="5c7a5-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto de teleconnector no corpo da resposta. [](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5c7a5-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c7a5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c7a5-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c7a5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7a5-128">Request</span></span>
<span data-ttu-id="5c7a5-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c7a5-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="5c7a5-130">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5c7a5-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5c7a5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c7a5-131">Response</span></span>
<span data-ttu-id="5c7a5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c7a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
