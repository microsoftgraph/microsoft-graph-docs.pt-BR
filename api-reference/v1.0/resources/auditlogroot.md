---
title: tipo de recurso auditLogRoot
description: Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades utilizáveis.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b8a90ae97c3ad1ff8c59ad9789c6b1c18498496
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889614"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="b9408-105">tipo de recurso auditLogRoot</span><span class="sxs-lookup"><span data-stu-id="b9408-105">auditLogRoot resource type</span></span>

<span data-ttu-id="b9408-106">Contém diferentes tipos de logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b9408-106">Contains different types of audit logs.</span></span> <span data-ttu-id="b9408-107">Esses recursos retornam um recurso singleton auditLog.</span><span class="sxs-lookup"><span data-stu-id="b9408-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="b9408-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="b9408-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b9408-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b9408-109">Methods</span></span>

| <span data-ttu-id="b9408-110">Método</span><span class="sxs-lookup"><span data-stu-id="b9408-110">Method</span></span>           | <span data-ttu-id="b9408-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b9408-111">Return Type</span></span>    |<span data-ttu-id="b9408-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9408-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9408-113">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="b9408-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="b9408-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b9408-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="b9408-115">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b9408-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="b9408-116">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b9408-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="b9408-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b9408-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="b9408-118">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b9408-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="b9408-119">Listar entrar</span><span class="sxs-lookup"><span data-stu-id="b9408-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="b9408-120">signIn</span><span class="sxs-lookup"><span data-stu-id="b9408-120">signIn</span></span>](signin.md) |<span data-ttu-id="b9408-121">Leia as propriedades e os relacionamentos de objetos de domínio.</span><span class="sxs-lookup"><span data-stu-id="b9408-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="b9408-122">Obter entrar</span><span class="sxs-lookup"><span data-stu-id="b9408-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="b9408-123">signIn</span><span class="sxs-lookup"><span data-stu-id="b9408-123">signIn</span></span>](signin.md) |<span data-ttu-id="b9408-124">Leia as propriedades e os relacionamentos de um objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="b9408-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9408-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9408-125">Properties</span></span>

<span data-ttu-id="b9408-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9408-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b9408-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b9408-127">Relationships</span></span>

| <span data-ttu-id="b9408-128">Relação</span><span class="sxs-lookup"><span data-stu-id="b9408-128">Relationship</span></span> | <span data-ttu-id="b9408-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9408-129">Type</span></span>   |<span data-ttu-id="b9408-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9408-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9408-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="b9408-131">directoryAudits</span></span>|<span data-ttu-id="b9408-132">coleção [directoryAudit](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="b9408-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="b9408-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9408-133">Read-only.</span></span> <span data-ttu-id="b9408-134">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9408-134">Nullable.</span></span>|
|<span data-ttu-id="b9408-135">signIns</span><span class="sxs-lookup"><span data-stu-id="b9408-135">signIns</span></span>|<span data-ttu-id="b9408-136">coleção de [entrada](signin.md)</span><span class="sxs-lookup"><span data-stu-id="b9408-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="b9408-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9408-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9408-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9408-139">JSON representation</span></span>

<span data-ttu-id="b9408-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9408-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b9408-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9408-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b9408-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9408-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9408-143">C#</span><span class="sxs-lookup"><span data-stu-id="b9408-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9408-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9408-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9408-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b9408-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b9408-146">Java</span><span class="sxs-lookup"><span data-stu-id="b9408-146">Java</span></span>](#tab/java)
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
