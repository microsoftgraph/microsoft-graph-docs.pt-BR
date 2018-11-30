---
title: Tipo de recurso FilterCriteria
description: Representa os critérios de filtragem aplicados a uma coluna.
ms.openlocfilehash: dbcc57ff940fec525b712eb11ac44209f5f8a4d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033836"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="8c32d-103">Tipo de recurso FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="8c32d-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="8c32d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c32d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c32d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c32d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c32d-106">Representa os critérios de filtragem aplicados a uma coluna.</span><span class="sxs-lookup"><span data-stu-id="8c32d-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c32d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c32d-107">JSON representation</span></span>

<span data-ttu-id="8c32d-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c32d-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```