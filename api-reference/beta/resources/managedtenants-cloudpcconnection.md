---
title: Tipo de recurso cloudPcConnection
description: Representa uma conexão de computador na nuvem para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 75af7be7633e43bc594f7185f196f40abca39883
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401946"
---
# <a name="cloudpcconnection-resource-type"></a><span data-ttu-id="7ed8a-103">Tipo de recurso cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="7ed8a-103">cloudPcConnection resource type</span></span>

<span data-ttu-id="7ed8a-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7ed8a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ed8a-105">Representa uma conexão de computador na nuvem para um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-105">Represents a cloud PC connection for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="7ed8a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ed8a-106">Methods</span></span>
|<span data-ttu-id="7ed8a-107">Método</span><span class="sxs-lookup"><span data-stu-id="7ed8a-107">Method</span></span>|<span data-ttu-id="7ed8a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ed8a-108">Return type</span></span>|<span data-ttu-id="7ed8a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed8a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ed8a-110">Listar cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="7ed8a-110">List cloudPcConnections</span></span>](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|<span data-ttu-id="7ed8a-111">[coleção microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8a-111">[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) collection</span></span>|<span data-ttu-id="7ed8a-112">Obter uma lista dos objetos [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-112">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>|
|[<span data-ttu-id="7ed8a-113">Obter cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="7ed8a-113">Get cloudPcConnection</span></span>](../api/managedtenants-cloudpcconnection-get.md)|[<span data-ttu-id="7ed8a-114">microsoft.graph.managedTenants.cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="7ed8a-114">microsoft.graph.managedTenants.cloudPcConnection</span></span>](../resources/managedtenants-cloudpcconnection.md)|<span data-ttu-id="7ed8a-115">Leia as propriedades e as relações de um [objeto cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8a-115">Read the properties and relationships of a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ed8a-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ed8a-116">Properties</span></span>
|<span data-ttu-id="7ed8a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ed8a-117">Property</span></span>|<span data-ttu-id="7ed8a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ed8a-118">Type</span></span>|<span data-ttu-id="7ed8a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed8a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed8a-120">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed8a-120">displayName</span></span>|<span data-ttu-id="7ed8a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed8a-121">String</span></span>|<span data-ttu-id="7ed8a-122">O nome de exibição da conexão do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-122">The display name of the cloud PC connection.</span></span> <span data-ttu-id="7ed8a-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-123">Required.</span></span> <span data-ttu-id="7ed8a-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-124">Read-only.</span></span>|
|<span data-ttu-id="7ed8a-125">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="7ed8a-125">healthCheckStatus</span></span>|<span data-ttu-id="7ed8a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed8a-126">String</span></span>|<span data-ttu-id="7ed8a-127">O status de saúde da conexão do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-127">The health status of the cloud PC connection.</span></span> <span data-ttu-id="7ed8a-128">Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-128">Possible values are: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span></span>  <span data-ttu-id="7ed8a-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-129">Required.</span></span> <span data-ttu-id="7ed8a-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-130">Read-only.</span></span>|
|<span data-ttu-id="7ed8a-131">id</span><span class="sxs-lookup"><span data-stu-id="7ed8a-131">id</span></span>|<span data-ttu-id="7ed8a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed8a-132">String</span></span>|<span data-ttu-id="7ed8a-133">O identificador exclusivo para a conexão de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-133">The unique identifier for the cloud PC connection.</span></span> <span data-ttu-id="7ed8a-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-134">Required.</span></span> <span data-ttu-id="7ed8a-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-135">Read-only.</span></span>|
|<span data-ttu-id="7ed8a-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed8a-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="7ed8a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed8a-137">DateTimeOffset</span></span>|<span data-ttu-id="7ed8a-138">Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="7ed8a-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-139">Required.</span></span> <span data-ttu-id="7ed8a-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-140">Read-only.</span></span>|
|<span data-ttu-id="7ed8a-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="7ed8a-141">tenantDisplayName</span></span>|<span data-ttu-id="7ed8a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed8a-142">String</span></span>|<span data-ttu-id="7ed8a-143">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-143">The display name for the managed tenant.</span></span> <span data-ttu-id="7ed8a-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-144">Required.</span></span> <span data-ttu-id="7ed8a-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-145">Read-only.</span></span>|
|<span data-ttu-id="7ed8a-146">tenantId</span><span class="sxs-lookup"><span data-stu-id="7ed8a-146">tenantId</span></span>|<span data-ttu-id="7ed8a-147">String</span><span class="sxs-lookup"><span data-stu-id="7ed8a-147">String</span></span>|<span data-ttu-id="7ed8a-148">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8a-148">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="7ed8a-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-149">Required.</span></span> <span data-ttu-id="7ed8a-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ed8a-151">Relações</span><span class="sxs-lookup"><span data-stu-id="7ed8a-151">Relationships</span></span>
<span data-ttu-id="7ed8a-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ed8a-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ed8a-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ed8a-153">JSON representation</span></span>
<span data-ttu-id="7ed8a-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ed8a-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
