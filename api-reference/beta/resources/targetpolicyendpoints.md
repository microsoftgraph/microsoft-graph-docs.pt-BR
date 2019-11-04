---
title: tipo de recurso targetPolicyEndpoints
description: Representa as plataformas que estão sendo direcionadas para notificações do usuário.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 9c1911900f4945d6f4b75d62c62457791fbb5c6a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939464"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="806d1-103">tipo de recurso targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="806d1-103">targetPolicyEndpoints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="806d1-104">Representa as plataformas que podem ser direcionadas para receber notificações enviadas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="806d1-104">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="806d1-105">Eles incluem Windows, iOS, Android e Web.</span><span class="sxs-lookup"><span data-stu-id="806d1-105">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="806d1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="806d1-106">Properties</span></span>

| <span data-ttu-id="806d1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="806d1-107">Property</span></span>     | <span data-ttu-id="806d1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="806d1-108">Type</span></span>        | <span data-ttu-id="806d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="806d1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="806d1-110">platformTypes</span><span class="sxs-lookup"><span data-stu-id="806d1-110">platformTypes</span></span>|<span data-ttu-id="806d1-111">String collection</span><span class="sxs-lookup"><span data-stu-id="806d1-111">String collection</span></span>|<span data-ttu-id="806d1-112">Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas.</span><span class="sxs-lookup"><span data-stu-id="806d1-112">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="806d1-113">Os valores válidos `Windows`são `iOS`, `Android` e `WebPush`.</span><span class="sxs-lookup"><span data-stu-id="806d1-113">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="806d1-114">Por padrão, todos os tipos de ponto de extremidade de envio (Windows, iOS, Android e webpush) estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="806d1-114">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="806d1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="806d1-115">JSON representation</span></span>

<span data-ttu-id="806d1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="806d1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->