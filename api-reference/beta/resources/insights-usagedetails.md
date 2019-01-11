---
title: tipo de recurso usageDetails
description: Tipo complexo que contém as propriedades de itens usados. Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8729973c2393a918d26314ec3b27a2c68079dbfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858951"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="fff6c-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="fff6c-104">usageDetails resource type</span></span>

> <span data-ttu-id="fff6c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fff6c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fff6c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fff6c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fff6c-107">Tipo complexo que contém as propriedades de itens [usado](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="fff6c-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="fff6c-108">Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fff6c-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fff6c-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fff6c-109">JSON representation</span></span>

<span data-ttu-id="fff6c-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fff6c-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="fff6c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fff6c-111">Properties</span></span>

| <span data-ttu-id="fff6c-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fff6c-112">Property</span></span>              | <span data-ttu-id="fff6c-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="fff6c-113">Type</span></span>          | <span data-ttu-id="fff6c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="fff6c-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="fff6c-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="fff6c-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="fff6c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fff6c-116">DateTimeOffset</span></span>        | <span data-ttu-id="fff6c-117">A data e hora que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fff6c-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="fff6c-118">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fff6c-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fff6c-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fff6c-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="fff6c-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fff6c-120">Read-only.</span></span>                      |
| <span data-ttu-id="fff6c-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fff6c-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="fff6c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fff6c-122">DateTimeOffset</span></span>        | <span data-ttu-id="fff6c-123">A data e hora que o recurso da última modificação pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fff6c-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="fff6c-124">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fff6c-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fff6c-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fff6c-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="fff6c-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fff6c-126">Read-only.</span></span>       |
