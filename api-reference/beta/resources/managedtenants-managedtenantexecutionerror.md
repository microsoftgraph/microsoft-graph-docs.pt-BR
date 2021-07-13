---
title: Tipo de recurso managedTenantExecutionError
description: Representa uma exceção para uma operação de locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401905"
---
# <a name="managedtenantexecutionerror-resource-type"></a><span data-ttu-id="41d02-103">Tipo de recurso managedTenantExecutionError</span><span class="sxs-lookup"><span data-stu-id="41d02-103">managedTenantExecutionError resource type</span></span>

<span data-ttu-id="41d02-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="41d02-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41d02-105">Representa uma exceção para uma operação de locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="41d02-105">Represents an exception for a managed tenant operation.</span></span>

<span data-ttu-id="41d02-106">Herda de [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="41d02-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="41d02-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41d02-107">Properties</span></span>
|<span data-ttu-id="41d02-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41d02-108">Property</span></span>|<span data-ttu-id="41d02-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41d02-109">Type</span></span>|<span data-ttu-id="41d02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41d02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d02-111">erro</span><span class="sxs-lookup"><span data-stu-id="41d02-111">error</span></span>|<span data-ttu-id="41d02-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41d02-112">String</span></span>|<span data-ttu-id="41d02-113">A mensagem de erro da exceção.</span><span class="sxs-lookup"><span data-stu-id="41d02-113">The error message for the exception.</span></span> <span data-ttu-id="41d02-114">Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="41d02-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="41d02-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d02-115">Required.</span></span> <span data-ttu-id="41d02-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-116">Read-only.</span></span>|
|<span data-ttu-id="41d02-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="41d02-117">errorDetails</span></span>|<span data-ttu-id="41d02-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41d02-118">String</span></span>|<span data-ttu-id="41d02-119">Informações de erro adicionais para a exceção.</span><span class="sxs-lookup"><span data-stu-id="41d02-119">Additional error information for the exception.</span></span> <span data-ttu-id="41d02-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41d02-120">Optional.</span></span> <span data-ttu-id="41d02-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-121">Read-only.</span></span>|
|<span data-ttu-id="41d02-122">nodeId</span><span class="sxs-lookup"><span data-stu-id="41d02-122">nodeId</span></span>|<span data-ttu-id="41d02-123">Int32</span><span class="sxs-lookup"><span data-stu-id="41d02-123">Int32</span></span>|<span data-ttu-id="41d02-124">O identificador do nó onde ocorreu a exceção.</span><span class="sxs-lookup"><span data-stu-id="41d02-124">The node identifier where the exception occurred.</span></span> <span data-ttu-id="41d02-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d02-125">Required.</span></span> <span data-ttu-id="41d02-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-126">Read-only.</span></span>|
|<span data-ttu-id="41d02-127">rawToken</span><span class="sxs-lookup"><span data-stu-id="41d02-127">rawToken</span></span>|<span data-ttu-id="41d02-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41d02-128">String</span></span>|<span data-ttu-id="41d02-129">O token da exceção.</span><span class="sxs-lookup"><span data-stu-id="41d02-129">The token for the exception.</span></span> <span data-ttu-id="41d02-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41d02-130">Optional.</span></span> <span data-ttu-id="41d02-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-131">Read-only.</span></span>|
|<span data-ttu-id="41d02-132">statementIndex</span><span class="sxs-lookup"><span data-stu-id="41d02-132">statementIndex</span></span>|<span data-ttu-id="41d02-133">Int32</span><span class="sxs-lookup"><span data-stu-id="41d02-133">Int32</span></span>|<span data-ttu-id="41d02-134">O índice de instrução da exceção.</span><span class="sxs-lookup"><span data-stu-id="41d02-134">The statement index for the exception.</span></span> <span data-ttu-id="41d02-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d02-135">Required.</span></span> <span data-ttu-id="41d02-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-136">Read-only.</span></span>|
|<span data-ttu-id="41d02-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="41d02-137">tenantId</span></span>|<span data-ttu-id="41d02-138">String</span><span class="sxs-lookup"><span data-stu-id="41d02-138">String</span></span>|<span data-ttu-id="41d02-139">O Azure Active Directory de locatário do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="41d02-139">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="41d02-140">Herdado [de managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="41d02-140">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="41d02-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d02-141">Required.</span></span> <span data-ttu-id="41d02-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41d02-142">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41d02-143">Relações</span><span class="sxs-lookup"><span data-stu-id="41d02-143">Relationships</span></span>
<span data-ttu-id="41d02-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41d02-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41d02-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41d02-145">JSON representation</span></span>
<span data-ttu-id="41d02-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41d02-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
