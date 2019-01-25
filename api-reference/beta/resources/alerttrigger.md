---
title: tipo de recurso de alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: cda1dde9b22b9304fd412405758435be2f6143bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516312"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="be77d-104">tipo de recurso de alertTrigger</span><span class="sxs-lookup"><span data-stu-id="be77d-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be77d-105">Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="be77d-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="be77d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be77d-106">Properties</span></span>

| <span data-ttu-id="be77d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be77d-107">Property</span></span>   | <span data-ttu-id="be77d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="be77d-108">Type</span></span>|<span data-ttu-id="be77d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="be77d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be77d-110">name</span><span class="sxs-lookup"><span data-stu-id="be77d-110">name</span></span>|<span data-ttu-id="be77d-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be77d-111">String</span></span>|<span data-ttu-id="be77d-112">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="be77d-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="be77d-113">type</span><span class="sxs-lookup"><span data-stu-id="be77d-113">type</span></span>|<span data-ttu-id="be77d-114">String</span><span class="sxs-lookup"><span data-stu-id="be77d-114">String</span></span>|<span data-ttu-id="be77d-115">Tipo da propriedade no par de chave: valor de interpretação.</span><span class="sxs-lookup"><span data-stu-id="be77d-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="be77d-116">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="be77d-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="be77d-117">valor</span><span class="sxs-lookup"><span data-stu-id="be77d-117">value</span></span>|<span data-ttu-id="be77d-118">String</span><span class="sxs-lookup"><span data-stu-id="be77d-118">String</span></span>|<span data-ttu-id="be77d-119">Valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="be77d-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be77d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be77d-120">JSON representation</span></span>

<span data-ttu-id="be77d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be77d-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="be77d-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be77d-122">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/alerttrigger.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
