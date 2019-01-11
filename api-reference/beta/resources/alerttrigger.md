---
title: tipo de recurso de alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: e375538806f09f85539f7a03e31c8a1ae041afdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866644"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="b0c88-104">tipo de recurso de alertTrigger</span><span class="sxs-lookup"><span data-stu-id="b0c88-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="b0c88-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0c88-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0c88-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0c88-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0c88-107">Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="b0c88-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="b0c88-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c88-108">Properties</span></span>

| <span data-ttu-id="b0c88-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c88-109">Property</span></span>   | <span data-ttu-id="b0c88-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c88-110">Type</span></span>|<span data-ttu-id="b0c88-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c88-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c88-112">name</span><span class="sxs-lookup"><span data-stu-id="b0c88-112">name</span></span>|<span data-ttu-id="b0c88-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0c88-113">String</span></span>|<span data-ttu-id="b0c88-114">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="b0c88-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="b0c88-115">type</span><span class="sxs-lookup"><span data-stu-id="b0c88-115">type</span></span>|<span data-ttu-id="b0c88-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0c88-116">String</span></span>|<span data-ttu-id="b0c88-117">Tipo da propriedade no par de chave: valor de interpretação.</span><span class="sxs-lookup"><span data-stu-id="b0c88-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="b0c88-118">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="b0c88-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="b0c88-119">valor</span><span class="sxs-lookup"><span data-stu-id="b0c88-119">value</span></span>|<span data-ttu-id="b0c88-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0c88-120">String</span></span>|<span data-ttu-id="b0c88-121">Valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="b0c88-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0c88-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c88-122">JSON representation</span></span>

<span data-ttu-id="b0c88-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c88-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b0c88-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0c88-124">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
