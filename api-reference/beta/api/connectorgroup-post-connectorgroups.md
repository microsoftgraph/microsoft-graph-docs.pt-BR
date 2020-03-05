---
title: Criar um conector
description: Use esta API para criar um novo conector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 21cdb4ec3da098ed787c13a4b8c4c24244dd6c8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437305"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="d90e3-103">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="d90e3-103">Create connectorGroup</span></span>

<span data-ttu-id="d90e3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d90e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d90e3-105">Use esta API para criar um novo conector.</span><span class="sxs-lookup"><span data-stu-id="d90e3-105">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d90e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d90e3-106">Permissions</span></span>
<span data-ttu-id="d90e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d90e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d90e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d90e3-109">Permission type</span></span>      | <span data-ttu-id="d90e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d90e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d90e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d90e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d90e3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d90e3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d90e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d90e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d90e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d90e3-114">Not supported.</span></span>    |
|<span data-ttu-id="d90e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d90e3-115">Application</span></span> | <span data-ttu-id="d90e3-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d90e3-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d90e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d90e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="d90e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d90e3-118">Request headers</span></span>
| <span data-ttu-id="d90e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d90e3-119">Name</span></span>       | <span data-ttu-id="d90e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d90e3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d90e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d90e3-121">Authorization</span></span>  | <span data-ttu-id="d90e3-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="d90e3-122">Bearer.</span></span> <span data-ttu-id="d90e3-123">Requried</span><span class="sxs-lookup"><span data-stu-id="d90e3-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90e3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d90e3-124">Request body</span></span>
<span data-ttu-id="d90e3-125">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="d90e3-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d90e3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d90e3-126">Response</span></span>

<span data-ttu-id="d90e3-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d90e3-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90e3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d90e3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d90e3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d90e3-129">Request</span></span>
<span data-ttu-id="d90e3-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d90e3-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="d90e3-131">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="d90e3-131">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d90e3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d90e3-132">Response</span></span>
<span data-ttu-id="d90e3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d90e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
