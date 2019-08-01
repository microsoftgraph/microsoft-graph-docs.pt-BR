---
title: tipo de recurso auditLogRoot
description: Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades utilizáveis.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2956b933b5d7703300964a0d6fd2014287f5e0ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030048"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="942b6-105">tipo de recurso auditLogRoot</span><span class="sxs-lookup"><span data-stu-id="942b6-105">auditLogRoot resource type</span></span>

<span data-ttu-id="942b6-106">Contém diferentes tipos de logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="942b6-106">Contains different types of audit logs.</span></span> <span data-ttu-id="942b6-107">Esses recursos retornam um recurso singleton auditLog.</span><span class="sxs-lookup"><span data-stu-id="942b6-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="942b6-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="942b6-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="942b6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="942b6-109">Methods</span></span>

| <span data-ttu-id="942b6-110">Método</span><span class="sxs-lookup"><span data-stu-id="942b6-110">Method</span></span>           | <span data-ttu-id="942b6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="942b6-111">Return Type</span></span>    |<span data-ttu-id="942b6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="942b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="942b6-113">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="942b6-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="942b6-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="942b6-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="942b6-115">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="942b6-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="942b6-116">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="942b6-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="942b6-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="942b6-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="942b6-118">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="942b6-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="942b6-119">Listar entrar</span><span class="sxs-lookup"><span data-stu-id="942b6-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="942b6-120">signIn</span><span class="sxs-lookup"><span data-stu-id="942b6-120">signIn</span></span>](signin.md) |<span data-ttu-id="942b6-121">Leia as propriedades e os relacionamentos de objetos de domínio.</span><span class="sxs-lookup"><span data-stu-id="942b6-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="942b6-122">Obter entrar</span><span class="sxs-lookup"><span data-stu-id="942b6-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="942b6-123">signIn</span><span class="sxs-lookup"><span data-stu-id="942b6-123">signIn</span></span>](signin.md) |<span data-ttu-id="942b6-124">Leia as propriedades e os relacionamentos de um objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="942b6-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="942b6-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="942b6-125">Properties</span></span>

<span data-ttu-id="942b6-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="942b6-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="942b6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="942b6-127">Relationships</span></span>

| <span data-ttu-id="942b6-128">Relação</span><span class="sxs-lookup"><span data-stu-id="942b6-128">Relationship</span></span> | <span data-ttu-id="942b6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="942b6-129">Type</span></span>   |<span data-ttu-id="942b6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="942b6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="942b6-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="942b6-131">directoryAudits</span></span>|<span data-ttu-id="942b6-132">coleção [directoryAudit](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="942b6-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="942b6-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="942b6-133">Read-only.</span></span> <span data-ttu-id="942b6-134">Anulável.</span><span class="sxs-lookup"><span data-stu-id="942b6-134">Nullable.</span></span>|
|<span data-ttu-id="942b6-135">signIns</span><span class="sxs-lookup"><span data-stu-id="942b6-135">signIns</span></span>|<span data-ttu-id="942b6-136">coleção de [entrada](signin.md)</span><span class="sxs-lookup"><span data-stu-id="942b6-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="942b6-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="942b6-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="942b6-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="942b6-139">JSON representation</span></span>

<span data-ttu-id="942b6-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="942b6-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="942b6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="942b6-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="942b6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="942b6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="942b6-143">C#</span><span class="sxs-lookup"><span data-stu-id="942b6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="942b6-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="942b6-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="942b6-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="942b6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="942b6-146">Java</span><span class="sxs-lookup"><span data-stu-id="942b6-146">Java</span></span>](#tab/java)
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
