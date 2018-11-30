---
title: tipo de recurso de segurança
description: O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança. Ele retornará um recurso de segurança único. Não contém todas as propriedades utilizáveis.
ms.openlocfilehash: ddf00e46135733ef18c18918c0c365134138671f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004364"
---
# <a name="security-resource-type"></a><span data-ttu-id="0db73-105">tipo de recurso de segurança</span><span class="sxs-lookup"><span data-stu-id="0db73-105">security resource type</span></span>

<span data-ttu-id="0db73-106">O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança.</span><span class="sxs-lookup"><span data-stu-id="0db73-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="0db73-107">Ele retornará um recurso de segurança único.</span><span class="sxs-lookup"><span data-stu-id="0db73-107">It returns a singleton security resource.</span></span> <span data-ttu-id="0db73-108">Não contém todas as propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="0db73-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="0db73-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0db73-109">Methods</span></span>

| <span data-ttu-id="0db73-110">Método</span><span class="sxs-lookup"><span data-stu-id="0db73-110">Method</span></span>       | <span data-ttu-id="0db73-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0db73-111">Return Type</span></span> | <span data-ttu-id="0db73-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db73-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0db73-113">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="0db73-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="0db73-114">coleção de [alerta](alert.md)</span><span class="sxs-lookup"><span data-stu-id="0db73-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="0db73-115">Obtenha uma coleção de objetos de alerta.</span><span class="sxs-lookup"><span data-stu-id="0db73-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="0db73-116">obter alertas</span><span class="sxs-lookup"><span data-stu-id="0db73-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="0db73-117">coleção de [alerta](alert.md)</span><span class="sxs-lookup"><span data-stu-id="0db73-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="0db73-118">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="0db73-118">Get a alert object.</span></span> |
| [<span data-ttu-id="0db73-119">Atualizar alertas</span><span class="sxs-lookup"><span data-stu-id="0db73-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="0db73-120">coleção de [alerta](alert.md)</span><span class="sxs-lookup"><span data-stu-id="0db73-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="0db73-121">Obter um objeto de alerta.</span><span class="sxs-lookup"><span data-stu-id="0db73-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0db73-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0db73-122">Properties</span></span>
<span data-ttu-id="0db73-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0db73-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0db73-124">Relações</span><span class="sxs-lookup"><span data-stu-id="0db73-124">Relationships</span></span>
| <span data-ttu-id="0db73-125">Relação</span><span class="sxs-lookup"><span data-stu-id="0db73-125">Relationship</span></span> | <span data-ttu-id="0db73-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0db73-126">Type</span></span>        | <span data-ttu-id="0db73-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db73-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0db73-128">alerts</span><span class="sxs-lookup"><span data-stu-id="0db73-128">alerts</span></span>|<span data-ttu-id="0db73-129">coleção de [alerta](alert.md)</span><span class="sxs-lookup"><span data-stu-id="0db73-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="0db73-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0db73-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0db73-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0db73-132">JSON representation</span></span>
<span data-ttu-id="0db73-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0db73-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="0db73-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0db73-134">Example</span></span>

<span data-ttu-id="0db73-135">O recurso de **segurança** está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="0db73-135">The **security** resource is available at the root of the graph.</span></span>

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