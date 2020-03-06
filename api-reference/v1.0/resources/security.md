---
title: tipo de recurso de segurança
description: O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança. Ele retorna um recurso de segurança singleton. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 89db6a8efbf50042e5514758ee5a7ae3b7f88de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533761"
---
# <a name="security-resource-type"></a><span data-ttu-id="eef2a-105">tipo de recurso de segurança</span><span class="sxs-lookup"><span data-stu-id="eef2a-105">security resource type</span></span>

<span data-ttu-id="eef2a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef2a-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eef2a-107">O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança.</span><span class="sxs-lookup"><span data-stu-id="eef2a-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="eef2a-108">Ele retorna um recurso de segurança singleton.</span><span class="sxs-lookup"><span data-stu-id="eef2a-108">It returns a singleton security resource.</span></span> <span data-ttu-id="eef2a-109">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="eef2a-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="eef2a-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="eef2a-110">Methods</span></span>

| <span data-ttu-id="eef2a-111">Método</span><span class="sxs-lookup"><span data-stu-id="eef2a-111">Method</span></span>       | <span data-ttu-id="eef2a-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eef2a-112">Return Type</span></span> | <span data-ttu-id="eef2a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef2a-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eef2a-114">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="eef2a-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="eef2a-115">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="eef2a-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="eef2a-116">Obtenha uma coleção de objetos de alerta.</span><span class="sxs-lookup"><span data-stu-id="eef2a-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="eef2a-117">obter alertas</span><span class="sxs-lookup"><span data-stu-id="eef2a-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="eef2a-118">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="eef2a-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="eef2a-119">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="eef2a-119">Get a alert object.</span></span> |
| [<span data-ttu-id="eef2a-120">Atualizar alertas</span><span class="sxs-lookup"><span data-stu-id="eef2a-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="eef2a-121">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="eef2a-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="eef2a-122">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="eef2a-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eef2a-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eef2a-123">Properties</span></span>
<span data-ttu-id="eef2a-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="eef2a-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="eef2a-125">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="eef2a-125">Relationships</span></span>
| <span data-ttu-id="eef2a-126">Relação</span><span class="sxs-lookup"><span data-stu-id="eef2a-126">Relationship</span></span> | <span data-ttu-id="eef2a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eef2a-127">Type</span></span>        | <span data-ttu-id="eef2a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef2a-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eef2a-129">alerts</span><span class="sxs-lookup"><span data-stu-id="eef2a-129">alerts</span></span>|<span data-ttu-id="eef2a-130">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="eef2a-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="eef2a-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="eef2a-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eef2a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eef2a-133">JSON representation</span></span>
<span data-ttu-id="eef2a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eef2a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="eef2a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eef2a-135">Example</span></span>

<span data-ttu-id="eef2a-136">O recurso de **segurança** está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="eef2a-136">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
