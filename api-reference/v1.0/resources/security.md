---
title: tipo de recurso de segurança
description: O recurso de segurança é o ponto de entrada para o modelo de objeto Security. Ele retorna um recurso de segurança singleton. Ele não contém propriedades usáveis.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 345e3e81b86fe42d16f4110450120c9f225c22dd
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473662"
---
# <a name="security-resource-type"></a><span data-ttu-id="66b69-105">tipo de recurso de segurança</span><span class="sxs-lookup"><span data-stu-id="66b69-105">security resource type</span></span>

<span data-ttu-id="66b69-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66b69-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66b69-107">O recurso de segurança é o ponto de entrada para o modelo de objeto Security.</span><span class="sxs-lookup"><span data-stu-id="66b69-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="66b69-108">Ele retorna um recurso de segurança singleton.</span><span class="sxs-lookup"><span data-stu-id="66b69-108">It returns a singleton security resource.</span></span> <span data-ttu-id="66b69-109">Ele não contém propriedades usáveis.</span><span class="sxs-lookup"><span data-stu-id="66b69-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="66b69-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="66b69-110">Methods</span></span>

| <span data-ttu-id="66b69-111">Método</span><span class="sxs-lookup"><span data-stu-id="66b69-111">Method</span></span>       | <span data-ttu-id="66b69-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66b69-112">Return Type</span></span> | <span data-ttu-id="66b69-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="66b69-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66b69-114">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="66b69-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="66b69-115">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="66b69-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="66b69-116">Obter uma coleção de objetos de alerta.</span><span class="sxs-lookup"><span data-stu-id="66b69-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="66b69-117">obter alertas</span><span class="sxs-lookup"><span data-stu-id="66b69-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="66b69-118">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="66b69-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="66b69-119">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="66b69-119">Get a alert object.</span></span> |
| [<span data-ttu-id="66b69-120">Atualizar alertas</span><span class="sxs-lookup"><span data-stu-id="66b69-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="66b69-121">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="66b69-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="66b69-122">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="66b69-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66b69-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66b69-123">Properties</span></span>
<span data-ttu-id="66b69-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="66b69-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="66b69-125">Relações</span><span class="sxs-lookup"><span data-stu-id="66b69-125">Relationships</span></span>
| <span data-ttu-id="66b69-126">Relação</span><span class="sxs-lookup"><span data-stu-id="66b69-126">Relationship</span></span> | <span data-ttu-id="66b69-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="66b69-127">Type</span></span>        | <span data-ttu-id="66b69-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="66b69-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66b69-129">alerts</span><span class="sxs-lookup"><span data-stu-id="66b69-129">alerts</span></span>|<span data-ttu-id="66b69-130">conjunto [alerta](alert.md) </span><span class="sxs-lookup"><span data-stu-id="66b69-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="66b69-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="66b69-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="66b69-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66b69-133">JSON representation</span></span>
<span data-ttu-id="66b69-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66b69-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="66b69-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66b69-135">Example</span></span>

<span data-ttu-id="66b69-136">O **recurso** de segurança está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="66b69-136">The **security** resource is available at the root of the graph.</span></span>

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
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

