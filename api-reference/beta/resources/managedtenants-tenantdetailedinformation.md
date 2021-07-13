---
title: Tipo de recurso tenantDetailedInformation
description: Representa informações detalhadas para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401994"
---
# <a name="tenantdetailedinformation-resource-type"></a><span data-ttu-id="05b38-103">Tipo de recurso tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="05b38-103">tenantDetailedInformation resource type</span></span>

<span data-ttu-id="05b38-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="05b38-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05b38-105">Representa informações detalhadas para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-105">Represents detailed information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="05b38-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="05b38-106">Methods</span></span>
|<span data-ttu-id="05b38-107">Método</span><span class="sxs-lookup"><span data-stu-id="05b38-107">Method</span></span>|<span data-ttu-id="05b38-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="05b38-108">Return type</span></span>|<span data-ttu-id="05b38-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05b38-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05b38-110">Listar tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="05b38-110">List tenantDetailedInformation</span></span>](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|<span data-ttu-id="05b38-111">[coleção microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="05b38-111">[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) collection</span></span>|<span data-ttu-id="05b38-112">Obter uma lista dos [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="05b38-112">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="05b38-113">Obter tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="05b38-113">Get tenantDetailedInformation</span></span>](../api/managedtenants-tenantdetailedinformation-get.md)|[<span data-ttu-id="05b38-114">microsoft.graph.managedTenants.tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="05b38-114">microsoft.graph.managedTenants.tenantDetailedInformation</span></span>](../resources/managedtenants-tenantdetailedinformation.md)|<span data-ttu-id="05b38-115">Leia as propriedades e as relações de um [objeto tenantDetailedInformation.](../resources/managedtenants-tenantdetailedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="05b38-115">Read the properties and relationships of a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05b38-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05b38-116">Properties</span></span>
|<span data-ttu-id="05b38-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05b38-117">Property</span></span>|<span data-ttu-id="05b38-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="05b38-118">Type</span></span>|<span data-ttu-id="05b38-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="05b38-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b38-120">city</span><span class="sxs-lookup"><span data-stu-id="05b38-120">city</span></span>|<span data-ttu-id="05b38-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-121">String</span></span>|<span data-ttu-id="05b38-122">A cidade onde o locatário gerenciado está localizado.</span><span class="sxs-lookup"><span data-stu-id="05b38-122">The city where the managed tenant is located.</span></span> <span data-ttu-id="05b38-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-123">Optional.</span></span> <span data-ttu-id="05b38-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-124">Read-only.</span></span>|
|<span data-ttu-id="05b38-125">countryCode</span><span class="sxs-lookup"><span data-stu-id="05b38-125">countryCode</span></span>|<span data-ttu-id="05b38-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-126">String</span></span>|<span data-ttu-id="05b38-127">O código do país onde o locatário gerenciado está localizado.</span><span class="sxs-lookup"><span data-stu-id="05b38-127">The code for the country where the managed tenant is located.</span></span> <span data-ttu-id="05b38-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-128">Optional.</span></span> <span data-ttu-id="05b38-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-129">Read-only.</span></span>|
|<span data-ttu-id="05b38-130">countryName</span><span class="sxs-lookup"><span data-stu-id="05b38-130">countryName</span></span>|<span data-ttu-id="05b38-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-131">String</span></span>|<span data-ttu-id="05b38-132">O nome do país onde o locatário gerenciado está localizado.</span><span class="sxs-lookup"><span data-stu-id="05b38-132">The name for the country where the managed tenant is located.</span></span> <span data-ttu-id="05b38-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-133">Optional.</span></span> <span data-ttu-id="05b38-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-134">Read-only.</span></span>|
|<span data-ttu-id="05b38-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="05b38-135">defaultDomainName</span></span>|<span data-ttu-id="05b38-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-136">String</span></span>|<span data-ttu-id="05b38-137">O nome de domínio padrão para o locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-137">The default domain name for the managed tenant.</span></span> <span data-ttu-id="05b38-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-138">Optional.</span></span> <span data-ttu-id="05b38-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-139">Read-only.</span></span>|
|<span data-ttu-id="05b38-140">displayName</span><span class="sxs-lookup"><span data-stu-id="05b38-140">displayName</span></span>|<span data-ttu-id="05b38-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-141">String</span></span>|<span data-ttu-id="05b38-142">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-142">The display name for the managed tenant.</span></span>|
|<span data-ttu-id="05b38-143">id</span><span class="sxs-lookup"><span data-stu-id="05b38-143">id</span></span>|<span data-ttu-id="05b38-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-144">String</span></span>|<span data-ttu-id="05b38-145">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="05b38-145">The unique identifier for this entity.</span></span> <span data-ttu-id="05b38-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05b38-146">Required.</span></span> <span data-ttu-id="05b38-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-147">Read-only.</span></span>|
|<span data-ttu-id="05b38-148">industryName</span><span class="sxs-lookup"><span data-stu-id="05b38-148">industryName</span></span>|<span data-ttu-id="05b38-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-149">String</span></span>|<span data-ttu-id="05b38-150">O setor comercial associado ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-150">The business industry associated with the managed tenant.</span></span> <span data-ttu-id="05b38-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-151">Optional.</span></span> <span data-ttu-id="05b38-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-152">Read-only.</span></span>|
|<span data-ttu-id="05b38-153">region</span><span class="sxs-lookup"><span data-stu-id="05b38-153">region</span></span>|<span data-ttu-id="05b38-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-154">String</span></span>|<span data-ttu-id="05b38-155">A região onde o locatário gerenciado está localizado.</span><span class="sxs-lookup"><span data-stu-id="05b38-155">The region where the managed tenant is located.</span></span> <span data-ttu-id="05b38-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-156">Optional.</span></span> <span data-ttu-id="05b38-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-157">Read-only.</span></span>|
|<span data-ttu-id="05b38-158">segmentName</span><span class="sxs-lookup"><span data-stu-id="05b38-158">segmentName</span></span>|<span data-ttu-id="05b38-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-159">String</span></span>|<span data-ttu-id="05b38-160">O segmento de negócios associado ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-160">The business segment associated with the managed tenant.</span></span> <span data-ttu-id="05b38-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-161">Optional.</span></span> <span data-ttu-id="05b38-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-162">Read-only.</span></span>|
|<span data-ttu-id="05b38-163">tenantId</span><span class="sxs-lookup"><span data-stu-id="05b38-163">tenantId</span></span>|<span data-ttu-id="05b38-164">String</span><span class="sxs-lookup"><span data-stu-id="05b38-164">String</span></span>|<span data-ttu-id="05b38-165">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="05b38-165">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="05b38-166">verticalName</span><span class="sxs-lookup"><span data-stu-id="05b38-166">verticalName</span></span>|<span data-ttu-id="05b38-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b38-167">String</span></span>|<span data-ttu-id="05b38-168">A vertical associada ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05b38-168">The vertical associated with the managed tenant.</span></span> <span data-ttu-id="05b38-169">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b38-169">Optional.</span></span> <span data-ttu-id="05b38-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05b38-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05b38-171">Relações</span><span class="sxs-lookup"><span data-stu-id="05b38-171">Relationships</span></span>
<span data-ttu-id="05b38-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05b38-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05b38-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05b38-173">JSON representation</span></span>
<span data-ttu-id="05b38-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05b38-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```

