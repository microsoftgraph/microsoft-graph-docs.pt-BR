---
title: tipo de recurso targetPolicyEndpoints
description: Representa as plataformas que estão sendo direcionadas para notificações do usuário.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: daac7a8424666d3974512c1cc1b17ec8e6878d7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985661"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="1b4bd-103">tipo de recurso targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="1b4bd-103">targetPolicyEndpoints resource type</span></span>

<span data-ttu-id="1b4bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b4bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b4bd-105">Representa as plataformas que podem ser direcionadas para receber notificações enviadas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1b4bd-105">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="1b4bd-106">Eles incluem Windows, iOS, Android e Web.</span><span class="sxs-lookup"><span data-stu-id="1b4bd-106">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="1b4bd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b4bd-107">Properties</span></span>

| <span data-ttu-id="1b4bd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b4bd-108">Property</span></span>     | <span data-ttu-id="1b4bd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b4bd-109">Type</span></span>        | <span data-ttu-id="1b4bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b4bd-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b4bd-111">platformTypes</span><span class="sxs-lookup"><span data-stu-id="1b4bd-111">platformTypes</span></span>|<span data-ttu-id="1b4bd-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b4bd-112">String collection</span></span>|<span data-ttu-id="1b4bd-113">Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas.</span><span class="sxs-lookup"><span data-stu-id="1b4bd-113">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="1b4bd-114">Os valores válidos `Windows` são `iOS` , `Android` e `WebPush` .</span><span class="sxs-lookup"><span data-stu-id="1b4bd-114">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="1b4bd-115">Por padrão, todos os tipos de ponto de extremidade de envio (Windows, iOS, Android e webpush) estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="1b4bd-115">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b4bd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b4bd-116">JSON representation</span></span>

<span data-ttu-id="1b4bd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b4bd-117">The following is a JSON representation of the resource.</span></span>

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

