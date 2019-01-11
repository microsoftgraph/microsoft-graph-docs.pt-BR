---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 78e4d1aff2003cc6d23580f4e52b46667cf6a9e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841703"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="9453c-102">Tipo de recurso EditAction</span><span class="sxs-lookup"><span data-stu-id="9453c-102">EditAction resource type</span></span>

> <span data-ttu-id="9453c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9453c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9453c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9453c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9453c-105">A presença do recurso **EditAction** em uma [**itemActivity**][activity] indica que a atividade editou um item.</span><span class="sxs-lookup"><span data-stu-id="9453c-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="9453c-106">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="9453c-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9453c-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9453c-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="9453c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9453c-108">Properties</span></span>

<span data-ttu-id="9453c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9453c-109">None.</span></span> <span data-ttu-id="9453c-110">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="9453c-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="9453c-111">Comentários</span><span class="sxs-lookup"><span data-stu-id="9453c-111">Remarks</span></span>

<span data-ttu-id="9453c-112">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9453c-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction"
} -->
