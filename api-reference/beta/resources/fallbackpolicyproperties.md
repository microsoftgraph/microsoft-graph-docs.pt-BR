---
title: tipo de recurso fallbackPolicyProperties
description: 'Permite que a política de fallback seja especificada para notificações brutas de alta prioridade somente nos pontos de extremidade do iOS, com propriedades adicionais para especificar o tempo de espera de fallback (atraso) e o conteúdo de notificação Visual correspondente. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a3ce59a23b5aec6dd43b370c3b67e9439b11937e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938959"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="5db0f-103">tipo de recurso fallbackPolicyProperties</span><span class="sxs-lookup"><span data-stu-id="5db0f-103">fallbackPolicyProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db0f-104">Permite que a política de fallback seja especificada para notificações brutas de alta prioridade somente nos pontos de extremidade do iOS, com propriedades adicionais para especificar o tempo de espera de fallback (atraso) e o conteúdo de notificação Visual correspondente.</span><span class="sxs-lookup"><span data-stu-id="5db0f-104">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="5db0f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5db0f-105">Properties</span></span>

| <span data-ttu-id="5db0f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5db0f-106">Property</span></span>     | <span data-ttu-id="5db0f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5db0f-107">Type</span></span>        | <span data-ttu-id="5db0f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5db0f-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5db0f-109">platformTypes</span><span class="sxs-lookup"><span data-stu-id="5db0f-109">platformTypes</span></span> | <span data-ttu-id="5db0f-110">String collection</span><span class="sxs-lookup"><span data-stu-id="5db0f-110">String collection</span></span> | <span data-ttu-id="5db0f-111">Especifica as plataformas que um desenvolvedor deseja habilitar para o fallback de notificação de torradeira de leitura para leitura visual.</span><span class="sxs-lookup"><span data-stu-id="5db0f-111">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="5db0f-112">No momento, se **fallbackPolicy** for especificado, **targetPolicy. platformTypes** deve `iOS` incluir e opcionalmente outras plataformas.</span><span class="sxs-lookup"><span data-stu-id="5db0f-112">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="5db0f-113">Além disso, o **fallbackPolicy. endpointFallback. platformTypes** é necessário e a única plataforma suportada atualmente `iOS`.</span><span class="sxs-lookup"><span data-stu-id="5db0f-113">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="5db0f-114">fallbackDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="5db0f-114">fallbackDelayInSeconds</span></span> | <span data-ttu-id="5db0f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="5db0f-115">Int32</span></span> | <span data-ttu-id="5db0f-116">Esse atraso representa a quantidade de tempo que passará (em segundos) antes que uma notificação de notificação direta seja enviada como um fallback para cada usuário de assinatura de dispositivo iOS que não buscará a notificação bruta.</span><span class="sxs-lookup"><span data-stu-id="5db0f-116">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="5db0f-117">O valor deve estar entre 60 e 600.</span><span class="sxs-lookup"><span data-stu-id="5db0f-117">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="5db0f-118">visualContent</span><span class="sxs-lookup"><span data-stu-id="5db0f-118">visualContent</span></span> | [<span data-ttu-id="5db0f-119">visualproperties</span><span class="sxs-lookup"><span data-stu-id="5db0f-119">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="5db0f-120">O conteúdo visual de uma notificação de usuário de retorno de fallback e bruto para Visual no iOS.</span><span class="sxs-lookup"><span data-stu-id="5db0f-120">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="5db0f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5db0f-121">JSON representation</span></span>

<span data-ttu-id="5db0f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5db0f-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicyProperties",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"],
  "fallbackDelayInSeconds": 60,
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicyProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->