---
title: tipo de recurso de plannerPlanContextDetailsCollection
description: " o valor é o objeto plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 0020ff8e8fd0d2e8dfd783e282e2bd648c16ec6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828235"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="1b5d6-103">tipo de recurso de plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="1b5d6-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="1b5d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b5d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="1b5d6-106">O recurso de **plannerPlanContextDetailsCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="1b5d6-107">Este recurso é um tipo aberto e parte do objeto [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="1b5d6-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="1b5d6-108">O nome da propriedade no par de valor da propriedade é um identificador de aplicativo específico do contexto; o valor é o objeto [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="1b5d6-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="1b5d6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b5d6-109">Properties</span></span>
<span data-ttu-id="1b5d6-110">Propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="1b5d6-111">Nesse caso, o cliente deve usar um identificador distinto que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="1b5d6-112">Os valores de propriedade devem ser [plannerPlanContextDetails](plannerplancontextdetails.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="1b5d6-113">Com base nos OData, os nomes de propriedade tipos abertos não podem conter os seguintes caracteres: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="1b5d6-114">Esses caracteres precisam ser codificada com o formato de codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="1b5d6-115">Para remover um item na lista Favoritos, o valor deve ser removido da coleção [plannerPlanContextCollection](plannerplancontextcollection.md) em vez disso, que removerá automaticamente a entrada neste objeto.</span><span class="sxs-lookup"><span data-stu-id="1b5d6-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
