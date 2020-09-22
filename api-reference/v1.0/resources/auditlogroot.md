---
title: tipo de recurso auditLogRoot
description: Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades utilizáveis.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86ecd0e7721ad804174359baf19bfde7a3230c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009447"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="3728b-105">tipo de recurso auditLogRoot</span><span class="sxs-lookup"><span data-stu-id="3728b-105">auditLogRoot resource type</span></span>

<span data-ttu-id="3728b-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3728b-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3728b-107">Contém diferentes tipos de logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3728b-107">Contains different types of audit logs.</span></span> <span data-ttu-id="3728b-108">Esses recursos retornam um recurso singleton auditLog.</span><span class="sxs-lookup"><span data-stu-id="3728b-108">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="3728b-109">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="3728b-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3728b-110">Methods</span><span class="sxs-lookup"><span data-stu-id="3728b-110">Methods</span></span>

| <span data-ttu-id="3728b-111">Método</span><span class="sxs-lookup"><span data-stu-id="3728b-111">Method</span></span>           | <span data-ttu-id="3728b-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3728b-112">Return Type</span></span>    |<span data-ttu-id="3728b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3728b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3728b-114">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="3728b-114">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="3728b-115">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="3728b-115">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="3728b-116">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3728b-116">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="3728b-117">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="3728b-117">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="3728b-118">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="3728b-118">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="3728b-119">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3728b-119">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="3728b-120">Listar entrar</span><span class="sxs-lookup"><span data-stu-id="3728b-120">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="3728b-121">signIn</span><span class="sxs-lookup"><span data-stu-id="3728b-121">signIn</span></span>](signin.md) |<span data-ttu-id="3728b-122">Leia as propriedades e os relacionamentos de objetos de domínio.</span><span class="sxs-lookup"><span data-stu-id="3728b-122">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="3728b-123">Obter entrar</span><span class="sxs-lookup"><span data-stu-id="3728b-123">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="3728b-124">signIn</span><span class="sxs-lookup"><span data-stu-id="3728b-124">signIn</span></span>](signin.md) |<span data-ttu-id="3728b-125">Leia as propriedades e os relacionamentos de um objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="3728b-125">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3728b-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3728b-126">Properties</span></span>

<span data-ttu-id="3728b-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3728b-127">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="3728b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3728b-128">Relationships</span></span>

| <span data-ttu-id="3728b-129">Relação</span><span class="sxs-lookup"><span data-stu-id="3728b-129">Relationship</span></span> | <span data-ttu-id="3728b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3728b-130">Type</span></span>   |<span data-ttu-id="3728b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3728b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3728b-132">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="3728b-132">directoryAudits</span></span>|<span data-ttu-id="3728b-133">coleção [directoryAudit](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="3728b-133">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="3728b-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3728b-134">Read-only.</span></span> <span data-ttu-id="3728b-135">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3728b-135">Nullable.</span></span>|
|<span data-ttu-id="3728b-136">signIns</span><span class="sxs-lookup"><span data-stu-id="3728b-136">signIns</span></span>|<span data-ttu-id="3728b-137">coleção de [entrada](signin.md)</span><span class="sxs-lookup"><span data-stu-id="3728b-137">[signIn](signin.md) collection</span></span>| <span data-ttu-id="3728b-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3728b-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3728b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3728b-140">JSON representation</span></span>

<span data-ttu-id="3728b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3728b-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="3728b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3728b-142">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="3728b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3728b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="c"></a>[<span data-ttu-id="3728b-144">C#</span><span class="sxs-lookup"><span data-stu-id="3728b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3728b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3728b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3728b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3728b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3728b-147">Java</span><span class="sxs-lookup"><span data-stu-id="3728b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

