---
title: Tipo de recurso managedTenantOperationError
description: Um tipo abstrato que representa um erro para uma operação de locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d8dc51747ac63f6f8a719b0256c398d14d1c4034
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402012"
---
# <a name="managedtenantoperationerror-resource-type"></a><span data-ttu-id="7eca2-103">Tipo de recurso managedTenantOperationError</span><span class="sxs-lookup"><span data-stu-id="7eca2-103">managedTenantOperationError resource type</span></span>

<span data-ttu-id="7eca2-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7eca2-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eca2-105">Um tipo abstrato que representa um erro para uma operação de locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7eca2-105">An abstract type that represents an error for a managed tenant operation.</span></span>

## <a name="properties"></a><span data-ttu-id="7eca2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7eca2-106">Properties</span></span>
|<span data-ttu-id="7eca2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7eca2-107">Property</span></span>|<span data-ttu-id="7eca2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eca2-108">Type</span></span>|<span data-ttu-id="7eca2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eca2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eca2-110">erro</span><span class="sxs-lookup"><span data-stu-id="7eca2-110">error</span></span>|<span data-ttu-id="7eca2-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7eca2-111">String</span></span>|<span data-ttu-id="7eca2-112">A mensagem de erro da exceção.</span><span class="sxs-lookup"><span data-stu-id="7eca2-112">The error message for the exception.</span></span>|
|<span data-ttu-id="7eca2-113">tenantId</span><span class="sxs-lookup"><span data-stu-id="7eca2-113">tenantId</span></span>|<span data-ttu-id="7eca2-114">String</span><span class="sxs-lookup"><span data-stu-id="7eca2-114">String</span></span>|<span data-ttu-id="7eca2-115">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="7eca2-115">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eca2-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7eca2-116">Relationships</span></span>
<span data-ttu-id="7eca2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7eca2-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eca2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7eca2-118">JSON representation</span></span>
<span data-ttu-id="7eca2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7eca2-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantOperationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantOperationError",
  "tenantId": "String",
  "error": "String"
}
```
