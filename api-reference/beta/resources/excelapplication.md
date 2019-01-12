---
title: Tipo de recurso de aplicativo
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921973"
---
# <a name="application-resource-type"></a><span data-ttu-id="f00f6-103">Tipo de recurso de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f00f6-103">Application resource type</span></span>

> <span data-ttu-id="f00f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f00f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f00f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f00f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f00f6-106">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f00f6-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="f00f6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f00f6-107">Methods</span></span>

| <span data-ttu-id="f00f6-108">Método</span><span class="sxs-lookup"><span data-stu-id="f00f6-108">Method</span></span>           | <span data-ttu-id="f00f6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f00f6-109">Return Type</span></span>    |<span data-ttu-id="f00f6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f00f6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f00f6-111">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="f00f6-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="f00f6-112">Application</span><span class="sxs-lookup"><span data-stu-id="f00f6-112">Application</span></span>](application.md) |<span data-ttu-id="f00f6-113">Leia as propriedades e os relacionamentos do objeto application.</span><span class="sxs-lookup"><span data-stu-id="f00f6-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="f00f6-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="f00f6-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="f00f6-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f00f6-115">None</span></span>|<span data-ttu-id="f00f6-116">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="f00f6-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="f00f6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f00f6-117">Properties</span></span>
| <span data-ttu-id="f00f6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f00f6-118">Property</span></span>     | <span data-ttu-id="f00f6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f00f6-119">Type</span></span>   |<span data-ttu-id="f00f6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f00f6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f00f6-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="f00f6-121">calculationMode</span></span>|<span data-ttu-id="f00f6-122">string</span><span class="sxs-lookup"><span data-stu-id="f00f6-122">string</span></span>|<span data-ttu-id="f00f6-123">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f00f6-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="f00f6-124">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="f00f6-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="f00f6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f00f6-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f00f6-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f00f6-126">Relationships</span></span>
<span data-ttu-id="f00f6-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f00f6-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f00f6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f00f6-128">JSON representation</span></span>

<span data-ttu-id="f00f6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f00f6-129">Here is a JSON representation of the resource.</span></span>

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
