---
title: tipo de recurso alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 594061ff17f80bb1ab462647562947b16965d9dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067388"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="2883d-104">tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="2883d-104">alertTrigger resource type</span></span>

<span data-ttu-id="2883d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2883d-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2883d-106">Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="2883d-106">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="2883d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2883d-107">Properties</span></span>

| <span data-ttu-id="2883d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2883d-108">Property</span></span>   | <span data-ttu-id="2883d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2883d-109">Type</span></span>|<span data-ttu-id="2883d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2883d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2883d-111">name</span><span class="sxs-lookup"><span data-stu-id="2883d-111">name</span></span>|<span data-ttu-id="2883d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2883d-112">String</span></span>|<span data-ttu-id="2883d-113">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="2883d-113">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="2883d-114">tipo</span><span class="sxs-lookup"><span data-stu-id="2883d-114">type</span></span>|<span data-ttu-id="2883d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2883d-115">String</span></span>|<span data-ttu-id="2883d-116">Tipo da propriedade no par chave: valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="2883d-116">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="2883d-117">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="2883d-117">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="2883d-118">value</span><span class="sxs-lookup"><span data-stu-id="2883d-118">value</span></span>|<span data-ttu-id="2883d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2883d-119">String</span></span>|<span data-ttu-id="2883d-120">O valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="2883d-120">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2883d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2883d-121">JSON representation</span></span>

<span data-ttu-id="2883d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2883d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="2883d-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2883d-123">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


