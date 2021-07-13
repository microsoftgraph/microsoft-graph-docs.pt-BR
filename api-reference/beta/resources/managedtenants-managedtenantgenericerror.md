---
title: Tipo de recurso managedTenantGenericError
description: Representa um erro genérico para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401899"
---
# <a name="managedtenantgenericerror-resource-type"></a><span data-ttu-id="b4380-103">Tipo de recurso managedTenantGenericError</span><span class="sxs-lookup"><span data-stu-id="b4380-103">managedTenantGenericError resource type</span></span>

<span data-ttu-id="b4380-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b4380-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4380-105">Representa um erro genérico para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b4380-105">Represents a generic error for a managed tenant.</span></span>

<span data-ttu-id="b4380-106">Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="b4380-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4380-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4380-107">Properties</span></span>
|<span data-ttu-id="b4380-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4380-108">Property</span></span>|<span data-ttu-id="b4380-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4380-109">Type</span></span>|<span data-ttu-id="b4380-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4380-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4380-111">erro</span><span class="sxs-lookup"><span data-stu-id="b4380-111">error</span></span>|<span data-ttu-id="b4380-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4380-112">String</span></span>|<span data-ttu-id="b4380-113">A mensagem de erro da exceção.</span><span class="sxs-lookup"><span data-stu-id="b4380-113">The error message for the exception.</span></span> <span data-ttu-id="b4380-114">Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="b4380-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="b4380-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4380-115">Required.</span></span> <span data-ttu-id="b4380-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4380-116">Read-only.</span></span>|
|<span data-ttu-id="b4380-117">tenantId</span><span class="sxs-lookup"><span data-stu-id="b4380-117">tenantId</span></span>|<span data-ttu-id="b4380-118">String</span><span class="sxs-lookup"><span data-stu-id="b4380-118">String</span></span>|<span data-ttu-id="b4380-119">O Azure Active Directory de locatário do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b4380-119">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="b4380-120">Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="b4380-120">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="b4380-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4380-121">Optional.</span></span> <span data-ttu-id="b4380-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4380-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4380-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b4380-123">Relationships</span></span>
<span data-ttu-id="b4380-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4380-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4380-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4380-125">JSON representation</span></span>
<span data-ttu-id="b4380-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4380-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
