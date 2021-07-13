---
title: Tipo de recurso tenantInfo
description: Representa informações para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c81df716b74511daab1f713f73bdd872e84e4987
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401992"
---
# <a name="tenantinfo-resource-type"></a><span data-ttu-id="e0d74-103">Tipo de recurso tenantInfo</span><span class="sxs-lookup"><span data-stu-id="e0d74-103">tenantInfo resource type</span></span>

<span data-ttu-id="e0d74-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e0d74-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0d74-105">Representa informações para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e0d74-105">Represents information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="e0d74-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0d74-106">Properties</span></span>
|<span data-ttu-id="e0d74-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0d74-107">Property</span></span>|<span data-ttu-id="e0d74-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0d74-108">Type</span></span>|<span data-ttu-id="e0d74-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0d74-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d74-110">tenantId</span><span class="sxs-lookup"><span data-stu-id="e0d74-110">tenantId</span></span>|<span data-ttu-id="e0d74-111">String</span><span class="sxs-lookup"><span data-stu-id="e0d74-111">String</span></span>|<span data-ttu-id="e0d74-112">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="e0d74-112">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="e0d74-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e0d74-113">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d74-114">Relações</span><span class="sxs-lookup"><span data-stu-id="e0d74-114">Relationships</span></span>
<span data-ttu-id="e0d74-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0d74-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0d74-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0d74-116">JSON representation</span></span>
<span data-ttu-id="e0d74-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0d74-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantInfo",
  "tenantId": "String"
}
```
