---
title: Tipo de recurso de aplicativo
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
ms.openlocfilehash: a8e2124910301818e753b1f90a3168da3a072862
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804435"
---
# <a name="application-resource-type"></a><span data-ttu-id="47854-103">Tipo de recurso de aplicativo</span><span class="sxs-lookup"><span data-stu-id="47854-103">Application resource type</span></span>

> <span data-ttu-id="47854-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47854-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47854-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47854-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47854-106">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="47854-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="47854-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="47854-107">Methods</span></span>

| <span data-ttu-id="47854-108">Método</span><span class="sxs-lookup"><span data-stu-id="47854-108">Method</span></span>           | <span data-ttu-id="47854-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="47854-109">Return Type</span></span>    |<span data-ttu-id="47854-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="47854-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47854-111">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="47854-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="47854-112">Application</span><span class="sxs-lookup"><span data-stu-id="47854-112">Application</span></span>](application.md) |<span data-ttu-id="47854-113">Leia as propriedades e os relacionamentos do objeto application.</span><span class="sxs-lookup"><span data-stu-id="47854-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="47854-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="47854-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="47854-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47854-115">None</span></span>|<span data-ttu-id="47854-116">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="47854-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="47854-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47854-117">Properties</span></span>
| <span data-ttu-id="47854-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47854-118">Property</span></span>     | <span data-ttu-id="47854-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="47854-119">Type</span></span>   |<span data-ttu-id="47854-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47854-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47854-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="47854-121">calculationMode</span></span>|<span data-ttu-id="47854-122">string</span><span class="sxs-lookup"><span data-stu-id="47854-122">string</span></span>|<span data-ttu-id="47854-123">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="47854-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="47854-124">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="47854-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="47854-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47854-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47854-126">Relações</span><span class="sxs-lookup"><span data-stu-id="47854-126">Relationships</span></span>
<span data-ttu-id="47854-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47854-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="47854-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47854-128">JSON representation</span></span>

<span data-ttu-id="47854-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47854-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
