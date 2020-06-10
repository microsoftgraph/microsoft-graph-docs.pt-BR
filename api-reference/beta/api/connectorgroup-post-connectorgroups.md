---
title: Criar um conector
description: Use esta API para criar um novo conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77d37dc53c963b2e5e1227d29cac49c0642768bd
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681233"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="c0dfe-103">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="c0dfe-103">Create connectorGroup</span></span>

<span data-ttu-id="c0dfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0dfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0dfe-105">Criar [um novo.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="c0dfe-105">Create a new [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0dfe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0dfe-106">Permissions</span></span>
<span data-ttu-id="c0dfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0dfe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0dfe-109">Permission type</span></span>      | <span data-ttu-id="c0dfe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0dfe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0dfe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0dfe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0dfe-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0dfe-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0dfe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0dfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0dfe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0dfe-114">Not supported.</span></span>    |
|<span data-ttu-id="c0dfe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0dfe-115">Application</span></span> | <span data-ttu-id="c0dfe-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0dfe-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0dfe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0dfe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="c0dfe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dfe-118">Request headers</span></span>
| <span data-ttu-id="c0dfe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c0dfe-119">Name</span></span>       | <span data-ttu-id="c0dfe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0dfe-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0dfe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0dfe-121">Authorization</span></span>  | <span data-ttu-id="c0dfe-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="c0dfe-122">Bearer.</span></span> <span data-ttu-id="c0dfe-123">Requried</span><span class="sxs-lookup"><span data-stu-id="c0dfe-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0dfe-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dfe-124">Request body</span></span>
<span data-ttu-id="c0dfe-125">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c0dfe-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0dfe-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0dfe-126">Response</span></span>

<span data-ttu-id="c0dfe-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0dfe-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0dfe-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0dfe-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0dfe-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dfe-129">Request</span></span>
<span data-ttu-id="c0dfe-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0dfe-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0dfe-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0dfe-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "isDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="c0dfe-132">C#</span><span class="sxs-lookup"><span data-stu-id="c0dfe-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0dfe-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0dfe-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0dfe-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0dfe-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c0dfe-135">No corpo da solicitação, forneça uma representação JSON do objeto do [conector](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c0dfe-135">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c0dfe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0dfe-136">Response</span></span>
<span data-ttu-id="c0dfe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0dfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
