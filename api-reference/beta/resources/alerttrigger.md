---
title: tipo de recurso alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: cda1dde9b22b9304fd412405758435be2f6143bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535691"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="930cd-104">tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="930cd-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="930cd-105">Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="930cd-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="930cd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="930cd-106">Properties</span></span>

| <span data-ttu-id="930cd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="930cd-107">Property</span></span>   | <span data-ttu-id="930cd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="930cd-108">Type</span></span>|<span data-ttu-id="930cd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="930cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="930cd-110">name</span><span class="sxs-lookup"><span data-stu-id="930cd-110">name</span></span>|<span data-ttu-id="930cd-111">String</span><span class="sxs-lookup"><span data-stu-id="930cd-111">String</span></span>|<span data-ttu-id="930cd-112">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="930cd-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="930cd-113">type</span><span class="sxs-lookup"><span data-stu-id="930cd-113">type</span></span>|<span data-ttu-id="930cd-114">String</span><span class="sxs-lookup"><span data-stu-id="930cd-114">String</span></span>|<span data-ttu-id="930cd-115">Tipo da propriedade no par chave: valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="930cd-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="930cd-116">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="930cd-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="930cd-117">value</span><span class="sxs-lookup"><span data-stu-id="930cd-117">value</span></span>|<span data-ttu-id="930cd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="930cd-118">String</span></span>|<span data-ttu-id="930cd-119">O valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="930cd-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="930cd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="930cd-120">JSON representation</span></span>

<span data-ttu-id="930cd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="930cd-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="930cd-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="930cd-122">Example</span></span>

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
