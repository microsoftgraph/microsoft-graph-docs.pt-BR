---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837251"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="29302-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="29302-103">provisionedPlan resource type</span></span>

> <span data-ttu-id="29302-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="29302-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29302-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="29302-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29302-106">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="29302-106">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="29302-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29302-107">Properties</span></span>
| <span data-ttu-id="29302-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29302-108">Property</span></span>     | <span data-ttu-id="29302-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="29302-109">Type</span></span>   |<span data-ttu-id="29302-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="29302-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29302-111">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="29302-111">capabilityStatus</span></span>|<span data-ttu-id="29302-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29302-112">String</span></span>|<span data-ttu-id="29302-113">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="29302-113">For example, “Enabled”.</span></span>|
|<span data-ttu-id="29302-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="29302-114">provisioningStatus</span></span>|<span data-ttu-id="29302-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29302-115">String</span></span>|<span data-ttu-id="29302-116">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="29302-116">For example, “Success”.</span></span>|
|<span data-ttu-id="29302-117">service</span><span class="sxs-lookup"><span data-stu-id="29302-117">service</span></span>|<span data-ttu-id="29302-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29302-118">String</span></span>|<span data-ttu-id="29302-119">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="29302-119">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29302-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29302-120">JSON representation</span></span>

<span data-ttu-id="29302-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="29302-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
