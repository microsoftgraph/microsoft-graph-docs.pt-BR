---
title: Tipo de recurso managedDeviceComplianceTrend
description: Representa uma tendência de dispositivos compatíveis e não compatíveis para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 70c3c84c5da6ffb2660a6289bc55c6ab3eef64be
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401939"
---
# <a name="manageddevicecompliancetrend-resource-type"></a><span data-ttu-id="d6676-103">Tipo de recurso managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="d6676-103">managedDeviceComplianceTrend resource type</span></span>

<span data-ttu-id="d6676-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d6676-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6676-105">Representa uma tendência de dispositivos compatíveis e não compatíveis para um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d6676-105">Represents a trend of compliant and non-compliant devices for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="d6676-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6676-106">Methods</span></span>
|<span data-ttu-id="d6676-107">Método</span><span class="sxs-lookup"><span data-stu-id="d6676-107">Method</span></span>|<span data-ttu-id="d6676-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6676-108">Return type</span></span>|<span data-ttu-id="d6676-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6676-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6676-110">Listar managedDeviceComplianceTrends</span><span class="sxs-lookup"><span data-stu-id="d6676-110">List managedDeviceComplianceTrends</span></span>](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|<span data-ttu-id="d6676-111">[Coleção microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="d6676-111">[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) collection</span></span>|<span data-ttu-id="d6676-112">Obter uma lista dos [objetos managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d6676-112">Get a list of the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d6676-113">Obter managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="d6676-113">Get managedDeviceComplianceTrend</span></span>](../api/managedtenants-manageddevicecompliancetrend-get.md)|[<span data-ttu-id="d6676-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="d6676-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span></span>](../resources/managedtenants-manageddevicecompliancetrend.md)|<span data-ttu-id="d6676-115">Leia as propriedades e as relações de [um objeto managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="d6676-115">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6676-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6676-116">Properties</span></span>
|<span data-ttu-id="d6676-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6676-117">Property</span></span>|<span data-ttu-id="d6676-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6676-118">Type</span></span>|<span data-ttu-id="d6676-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6676-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6676-120">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-120">compliantDeviceCount</span></span>|<span data-ttu-id="d6676-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-121">Int32</span></span>|<span data-ttu-id="d6676-122">O número de dispositivos com um status compatível.</span><span class="sxs-lookup"><span data-stu-id="d6676-122">The number of devices with a compliant status.</span></span> <span data-ttu-id="d6676-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-123">Required.</span></span> <span data-ttu-id="d6676-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-124">Read-only.</span></span>|
|<span data-ttu-id="d6676-125">configManagerDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-125">configManagerDeviceCount</span></span>|<span data-ttu-id="d6676-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-126">Int32</span></span>|<span data-ttu-id="d6676-127">O número de dispositivos maneados pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d6676-127">The number of devices manged by Configuration Manager.</span></span> <span data-ttu-id="d6676-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-128">Required.</span></span> <span data-ttu-id="d6676-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-129">Read-only.</span></span>|
|<span data-ttu-id="d6676-130">countDateTime</span><span class="sxs-lookup"><span data-stu-id="d6676-130">countDateTime</span></span>|<span data-ttu-id="d6676-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6676-131">String</span></span>|<span data-ttu-id="d6676-132">O instantâneo de conformidade de data e hora foi executado.</span><span class="sxs-lookup"><span data-stu-id="d6676-132">The date and time compliance snapshot was performed.</span></span> <span data-ttu-id="d6676-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-133">Required.</span></span> <span data-ttu-id="d6676-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-134">Read-only.</span></span>|
|<span data-ttu-id="d6676-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-135">errorDeviceCount</span></span>|<span data-ttu-id="d6676-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-136">Int32</span></span>|<span data-ttu-id="d6676-137">O número de dispositivos com um status de erro.</span><span class="sxs-lookup"><span data-stu-id="d6676-137">The number of devices with an error status.</span></span> <span data-ttu-id="d6676-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-138">Required.</span></span> <span data-ttu-id="d6676-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-139">Read-only.</span></span>|
|<span data-ttu-id="d6676-140">id</span><span class="sxs-lookup"><span data-stu-id="d6676-140">id</span></span>|<span data-ttu-id="d6676-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6676-141">String</span></span>|<span data-ttu-id="d6676-142">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="d6676-142">The unique identifier for this entity.</span></span> <span data-ttu-id="d6676-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-143">Required.</span></span> <span data-ttu-id="d6676-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-144">Read-only.</span></span>|
|<span data-ttu-id="d6676-145">inGracePeriodDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-145">inGracePeriodDeviceCount</span></span>|<span data-ttu-id="d6676-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-146">Int32</span></span>|<span data-ttu-id="d6676-147">O número de dispositivos que estão em um status de período de carência.</span><span class="sxs-lookup"><span data-stu-id="d6676-147">The number of devices that are in a grace period status.</span></span> <span data-ttu-id="d6676-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-148">Required.</span></span> <span data-ttu-id="d6676-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-149">Read-only.</span></span>|
|<span data-ttu-id="d6676-150">noncompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-150">noncompliantDeviceCount</span></span>|<span data-ttu-id="d6676-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-151">Int32</span></span>|<span data-ttu-id="d6676-152">O número de dispositivos que estão em um status não compatível.</span><span class="sxs-lookup"><span data-stu-id="d6676-152">The number of devices that are in a non-compliant status.</span></span> <span data-ttu-id="d6676-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-153">Required.</span></span> <span data-ttu-id="d6676-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-154">Read-only.</span></span>|
|<span data-ttu-id="d6676-155">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6676-155">tenantDisplayName</span></span>|<span data-ttu-id="d6676-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6676-156">String</span></span>|<span data-ttu-id="d6676-157">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d6676-157">The display name for the managed tenant.</span></span> <span data-ttu-id="d6676-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6676-158">Optional.</span></span> <span data-ttu-id="d6676-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-159">Read-only.</span></span>|
|<span data-ttu-id="d6676-160">tenantId</span><span class="sxs-lookup"><span data-stu-id="d6676-160">tenantId</span></span>|<span data-ttu-id="d6676-161">String</span><span class="sxs-lookup"><span data-stu-id="d6676-161">String</span></span>|<span data-ttu-id="d6676-162">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="d6676-162">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="d6676-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6676-163">Optional.</span></span> <span data-ttu-id="d6676-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-164">Read-only.</span></span>|
|<span data-ttu-id="d6676-165">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d6676-165">unknownDeviceCount</span></span>|<span data-ttu-id="d6676-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d6676-166">Int32</span></span>|<span data-ttu-id="d6676-167">O número de dispositivos em um status desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d6676-167">The number of devices in an unknown status.</span></span> <span data-ttu-id="d6676-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6676-168">Required.</span></span> <span data-ttu-id="d6676-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6676-169">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6676-170">Relações</span><span class="sxs-lookup"><span data-stu-id="d6676-170">Relationships</span></span>
<span data-ttu-id="d6676-171">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6676-171">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6676-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6676-172">JSON representation</span></span>
<span data-ttu-id="d6676-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6676-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```
