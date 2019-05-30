---
title: tipo de recurso auditLogRoot
description: Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades utilizáveis.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a0f961850e0ef48776cf708348fcbacf4c9642c3
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536033"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="cc51c-105">tipo de recurso auditLogRoot</span><span class="sxs-lookup"><span data-stu-id="cc51c-105">auditLogRoot resource type</span></span>

<span data-ttu-id="cc51c-106">Contém diferentes tipos de logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="cc51c-106">Contains different types of audit logs.</span></span> <span data-ttu-id="cc51c-107">Esses recursos retornam um recurso singleton auditLog.</span><span class="sxs-lookup"><span data-stu-id="cc51c-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="cc51c-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="cc51c-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="cc51c-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc51c-109">Methods</span></span>

| <span data-ttu-id="cc51c-110">Método</span><span class="sxs-lookup"><span data-stu-id="cc51c-110">Method</span></span>           | <span data-ttu-id="cc51c-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc51c-111">Return Type</span></span>    |<span data-ttu-id="cc51c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc51c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc51c-113">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="cc51c-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="cc51c-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="cc51c-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="cc51c-115">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cc51c-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="cc51c-116">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="cc51c-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="cc51c-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="cc51c-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="cc51c-118">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cc51c-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="cc51c-119">Listar entrar</span><span class="sxs-lookup"><span data-stu-id="cc51c-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="cc51c-120">signIn</span><span class="sxs-lookup"><span data-stu-id="cc51c-120">signIn</span></span>](signin.md) |<span data-ttu-id="cc51c-121">Leia as propriedades e os relacionamentos de objetos de domínio.</span><span class="sxs-lookup"><span data-stu-id="cc51c-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="cc51c-122">Obter entrar</span><span class="sxs-lookup"><span data-stu-id="cc51c-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="cc51c-123">signIn</span><span class="sxs-lookup"><span data-stu-id="cc51c-123">signIn</span></span>](signin.md) |<span data-ttu-id="cc51c-124">Leia as propriedades e os relacionamentos de um objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="cc51c-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc51c-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc51c-125">Properties</span></span>

<span data-ttu-id="cc51c-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc51c-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="cc51c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="cc51c-127">Relationships</span></span>

| <span data-ttu-id="cc51c-128">Relação</span><span class="sxs-lookup"><span data-stu-id="cc51c-128">Relationship</span></span> | <span data-ttu-id="cc51c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc51c-129">Type</span></span>   |<span data-ttu-id="cc51c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc51c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc51c-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="cc51c-131">directoryAudits</span></span>|<span data-ttu-id="cc51c-132">coleção [directoryAudit](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="cc51c-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="cc51c-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc51c-133">Read-only.</span></span> <span data-ttu-id="cc51c-134">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc51c-134">Nullable.</span></span>|
|<span data-ttu-id="cc51c-135">signIns</span><span class="sxs-lookup"><span data-stu-id="cc51c-135">signIns</span></span>|<span data-ttu-id="cc51c-136">coleção de [entrada](signin.md)</span><span class="sxs-lookup"><span data-stu-id="cc51c-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="cc51c-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc51c-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc51c-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc51c-139">JSON representation</span></span>

<span data-ttu-id="cc51c-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc51c-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="cc51c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc51c-141">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cc51c-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cc51c-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cc51c-143">C#</span><span class="sxs-lookup"><span data-stu-id="cc51c-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc51c-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc51c-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_auditLogs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
