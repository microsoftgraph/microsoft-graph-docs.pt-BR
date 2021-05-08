---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231833"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="89d36-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="89d36-105">educationTerm resource type</span></span>

<span data-ttu-id="89d36-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d36-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89d36-107">Termo A.</span><span class="sxs-lookup"><span data-stu-id="89d36-107">A term.</span></span> <span data-ttu-id="89d36-108">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="89d36-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="89d36-109">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="89d36-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="89d36-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89d36-110">Properties</span></span>

| <span data-ttu-id="89d36-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89d36-111">Property</span></span>    | <span data-ttu-id="89d36-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="89d36-112">Type</span></span>   | <span data-ttu-id="89d36-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="89d36-113">Description</span></span>                       |
| :---------- | :----- | :-------------------------------- |
| <span data-ttu-id="89d36-114">displayName</span><span class="sxs-lookup"><span data-stu-id="89d36-114">displayName</span></span> | <span data-ttu-id="89d36-115">String</span><span class="sxs-lookup"><span data-stu-id="89d36-115">String</span></span> | <span data-ttu-id="89d36-116">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="89d36-116">Display name of the term.</span></span>         |
| <span data-ttu-id="89d36-117">externalId</span><span class="sxs-lookup"><span data-stu-id="89d36-117">externalId</span></span>  | <span data-ttu-id="89d36-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89d36-118">String</span></span> | <span data-ttu-id="89d36-119">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="89d36-119">ID of term in the syncing system.</span></span> |
| <span data-ttu-id="89d36-120">startDate</span><span class="sxs-lookup"><span data-stu-id="89d36-120">startDate</span></span>   | <span data-ttu-id="89d36-121">Data</span><span class="sxs-lookup"><span data-stu-id="89d36-121">Date</span></span>   | <span data-ttu-id="89d36-122">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="89d36-122">Start of the term.</span></span>                |
| <span data-ttu-id="89d36-123">endDate</span><span class="sxs-lookup"><span data-stu-id="89d36-123">endDate</span></span>     | <span data-ttu-id="89d36-124">Data</span><span class="sxs-lookup"><span data-stu-id="89d36-124">Date</span></span>   | <span data-ttu-id="89d36-125">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="89d36-125">End of the term.</span></span>                  |

## <a name="relationships"></a><span data-ttu-id="89d36-126">Relações</span><span class="sxs-lookup"><span data-stu-id="89d36-126">Relationships</span></span>

<span data-ttu-id="89d36-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89d36-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89d36-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89d36-128">JSON representation</span></span>

<span data-ttu-id="89d36-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89d36-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
