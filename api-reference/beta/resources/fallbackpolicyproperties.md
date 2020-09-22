---
title: tipo de recurso fallbackPolicyProperties
description: 'Permite que a política de fallback seja especificada para notificações brutas de alta prioridade somente nos pontos de extremidade do iOS, com propriedades adicionais para especificar o tempo de espera de fallback (atraso) e o conteúdo de notificação Visual correspondente. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: ee32b40f71c2540bb06b8b4478d0f896aac40b85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071204"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="56eaf-103">tipo de recurso fallbackPolicyProperties</span><span class="sxs-lookup"><span data-stu-id="56eaf-103">fallbackPolicyProperties resource type</span></span>

<span data-ttu-id="56eaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56eaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56eaf-105">Permite que a política de fallback seja especificada para notificações brutas de alta prioridade somente nos pontos de extremidade do iOS, com propriedades adicionais para especificar o tempo de espera de fallback (atraso) e o conteúdo de notificação Visual correspondente.</span><span class="sxs-lookup"><span data-stu-id="56eaf-105">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="56eaf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56eaf-106">Properties</span></span>

| <span data-ttu-id="56eaf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56eaf-107">Property</span></span>     | <span data-ttu-id="56eaf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="56eaf-108">Type</span></span>        | <span data-ttu-id="56eaf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56eaf-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="56eaf-110">platformTypes</span><span class="sxs-lookup"><span data-stu-id="56eaf-110">platformTypes</span></span> | <span data-ttu-id="56eaf-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56eaf-111">String collection</span></span> | <span data-ttu-id="56eaf-112">Especifica as plataformas que um desenvolvedor deseja habilitar para o fallback de notificação de torradeira de leitura para leitura visual.</span><span class="sxs-lookup"><span data-stu-id="56eaf-112">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="56eaf-113">No momento, se **fallbackPolicy** for especificado, **targetPolicy. platformTypes** deve incluir `iOS` e opcionalmente outras plataformas.</span><span class="sxs-lookup"><span data-stu-id="56eaf-113">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="56eaf-114">Além disso, o **fallbackPolicy. endpointFallback. platformTypes** é necessário e a única plataforma suportada atualmente `iOS` .</span><span class="sxs-lookup"><span data-stu-id="56eaf-114">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="56eaf-115">fallbackDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="56eaf-115">fallbackDelayInSeconds</span></span> | <span data-ttu-id="56eaf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="56eaf-116">Int32</span></span> | <span data-ttu-id="56eaf-117">Esse atraso representa a quantidade de tempo que passará (em segundos) antes que uma notificação de notificação direta seja enviada como um fallback para cada usuário de assinatura de dispositivo iOS que não buscará a notificação bruta.</span><span class="sxs-lookup"><span data-stu-id="56eaf-117">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="56eaf-118">O valor deve estar entre 60 e 600.</span><span class="sxs-lookup"><span data-stu-id="56eaf-118">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="56eaf-119">visualContent</span><span class="sxs-lookup"><span data-stu-id="56eaf-119">visualContent</span></span> | [<span data-ttu-id="56eaf-120">visualproperties</span><span class="sxs-lookup"><span data-stu-id="56eaf-120">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="56eaf-121">O conteúdo visual de uma notificação de usuário de retorno de fallback e bruto para Visual no iOS.</span><span class="sxs-lookup"><span data-stu-id="56eaf-121">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="56eaf-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56eaf-122">JSON representation</span></span>

<span data-ttu-id="56eaf-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56eaf-123">The following is a JSON representation of the resource.</span></span>

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

