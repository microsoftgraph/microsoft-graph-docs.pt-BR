---
title: Tipo de recurso alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1cda08c26b5d28de4c2b57c2bb5b34f79a84bcd8
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129457"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="e5cd5-104">Tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="e5cd5-104">alertTrigger resource type</span></span>

<span data-ttu-id="e5cd5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5cd5-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5cd5-106">Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="e5cd5-106">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="e5cd5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5cd5-107">Properties</span></span>

| <span data-ttu-id="e5cd5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5cd5-108">Property</span></span>   | <span data-ttu-id="e5cd5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5cd5-109">Type</span></span>|<span data-ttu-id="e5cd5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5cd5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5cd5-111">nome</span><span class="sxs-lookup"><span data-stu-id="e5cd5-111">name</span></span>|<span data-ttu-id="e5cd5-112">String</span><span class="sxs-lookup"><span data-stu-id="e5cd5-112">String</span></span>|<span data-ttu-id="e5cd5-113">Nome da propriedade que serve como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="e5cd5-113">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="e5cd5-114">tipo</span><span class="sxs-lookup"><span data-stu-id="e5cd5-114">type</span></span>|<span data-ttu-id="e5cd5-115">String</span><span class="sxs-lookup"><span data-stu-id="e5cd5-115">String</span></span>|<span data-ttu-id="e5cd5-116">Tipo da propriedade no par key:value para interpretação.</span><span class="sxs-lookup"><span data-stu-id="e5cd5-116">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="e5cd5-117">Por exemplo, String, Boolean etc.</span><span class="sxs-lookup"><span data-stu-id="e5cd5-117">For example, String, Boolean etc.</span></span>|
|<span data-ttu-id="e5cd5-118">value</span><span class="sxs-lookup"><span data-stu-id="e5cd5-118">value</span></span>|<span data-ttu-id="e5cd5-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5cd5-119">String</span></span>|<span data-ttu-id="e5cd5-120">Valor da propriedade que serve como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="e5cd5-120">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5cd5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5cd5-121">JSON representation</span></span>

<span data-ttu-id="e5cd5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5cd5-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e5cd5-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5cd5-123">Example</span></span>

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


