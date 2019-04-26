---
title: tipo de recurso alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 9142c4d86b627f1d1e1e790c9b3b279b07005ad2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339152"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="83c6f-104">tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="83c6f-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83c6f-105">Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="83c6f-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="83c6f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83c6f-106">Properties</span></span>

| <span data-ttu-id="83c6f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83c6f-107">Property</span></span>   | <span data-ttu-id="83c6f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="83c6f-108">Type</span></span>|<span data-ttu-id="83c6f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="83c6f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83c6f-110">name</span><span class="sxs-lookup"><span data-stu-id="83c6f-110">name</span></span>|<span data-ttu-id="83c6f-111">String</span><span class="sxs-lookup"><span data-stu-id="83c6f-111">String</span></span>|<span data-ttu-id="83c6f-112">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="83c6f-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="83c6f-113">type</span><span class="sxs-lookup"><span data-stu-id="83c6f-113">type</span></span>|<span data-ttu-id="83c6f-114">String</span><span class="sxs-lookup"><span data-stu-id="83c6f-114">String</span></span>|<span data-ttu-id="83c6f-115">Tipo da propriedade no par chave: valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="83c6f-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="83c6f-116">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="83c6f-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="83c6f-117">value</span><span class="sxs-lookup"><span data-stu-id="83c6f-117">value</span></span>|<span data-ttu-id="83c6f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83c6f-118">String</span></span>|<span data-ttu-id="83c6f-119">O valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="83c6f-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83c6f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83c6f-120">JSON representation</span></span>

<span data-ttu-id="83c6f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83c6f-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="83c6f-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83c6f-122">Example</span></span>

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
