---
title: Tipo de recurso tenantCustomizedInformation
description: Representa informações personalizáveis para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 580479e6fd710eef7a0907ea51cd5605ef445e40
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402137"
---
# <a name="tenantcustomizedinformation-resource-type"></a><span data-ttu-id="b03ac-103">Tipo de recurso tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="b03ac-103">tenantCustomizedInformation resource type</span></span>

<span data-ttu-id="b03ac-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b03ac-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b03ac-105">Representa informações personalizáveis para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b03ac-105">Represents customizable information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="b03ac-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b03ac-106">Methods</span></span>
|<span data-ttu-id="b03ac-107">Método</span><span class="sxs-lookup"><span data-stu-id="b03ac-107">Method</span></span>|<span data-ttu-id="b03ac-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b03ac-108">Return type</span></span>|<span data-ttu-id="b03ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03ac-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b03ac-110">Listar tenantCustomizedInformations</span><span class="sxs-lookup"><span data-stu-id="b03ac-110">List tenantCustomizedInformations</span></span>](../api/managedtenants-managedtenant-list-tenantscustomizedinformation.md)|<span data-ttu-id="b03ac-111">[coleção microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b03ac-111">[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection</span></span>|<span data-ttu-id="b03ac-112">Obter uma lista dos [objetos tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b03ac-112">Get a list of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="b03ac-113">Obter tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="b03ac-113">Get tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-get.md)|[<span data-ttu-id="b03ac-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="b03ac-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="b03ac-115">Leia as propriedades e as relações de um [objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b03ac-115">Read the properties and relationships of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|
|[<span data-ttu-id="b03ac-116">Atualizar tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="b03ac-116">Update tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-update.md)|[<span data-ttu-id="b03ac-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="b03ac-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="b03ac-118">Atualize as propriedades de [um objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b03ac-118">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b03ac-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b03ac-119">Properties</span></span>
|<span data-ttu-id="b03ac-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b03ac-120">Property</span></span>|<span data-ttu-id="b03ac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b03ac-121">Type</span></span>|<span data-ttu-id="b03ac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03ac-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b03ac-123">contacts</span><span class="sxs-lookup"><span data-stu-id="b03ac-123">contacts</span></span>|<span data-ttu-id="b03ac-124">[coleção microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b03ac-124">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="b03ac-125">A coleção de contatos do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b03ac-125">The collection of contacts for the managed tenant.</span></span> <span data-ttu-id="b03ac-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b03ac-126">Optional.</span></span>|
|<span data-ttu-id="b03ac-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b03ac-127">displayName</span></span>|<span data-ttu-id="b03ac-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b03ac-128">String</span></span>|<span data-ttu-id="b03ac-129">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b03ac-129">The display name for the managed tenant.</span></span> <span data-ttu-id="b03ac-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03ac-130">Required.</span></span> <span data-ttu-id="b03ac-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b03ac-131">Read-only.</span></span>|
|<span data-ttu-id="b03ac-132">id</span><span class="sxs-lookup"><span data-stu-id="b03ac-132">id</span></span>|<span data-ttu-id="b03ac-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b03ac-133">String</span></span>|<span data-ttu-id="b03ac-134">O Azure Active Directory de locatário do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b03ac-134">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="b03ac-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03ac-135">Required.</span></span> <span data-ttu-id="b03ac-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b03ac-136">Read-only.</span></span>|
|<span data-ttu-id="b03ac-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="b03ac-137">tenantId</span></span>|<span data-ttu-id="b03ac-138">String</span><span class="sxs-lookup"><span data-stu-id="b03ac-138">String</span></span>|<span data-ttu-id="b03ac-139">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="b03ac-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="b03ac-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b03ac-140">Optional.</span></span> <span data-ttu-id="b03ac-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b03ac-141">Read-only.</span></span>|
|<span data-ttu-id="b03ac-142">site</span><span class="sxs-lookup"><span data-stu-id="b03ac-142">website</span></span>|<span data-ttu-id="b03ac-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b03ac-143">String</span></span>|<span data-ttu-id="b03ac-144">O site do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b03ac-144">The website for the managed tenant.</span></span> <span data-ttu-id="b03ac-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03ac-145">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b03ac-146">Relações</span><span class="sxs-lookup"><span data-stu-id="b03ac-146">Relationships</span></span>
<span data-ttu-id="b03ac-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b03ac-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b03ac-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b03ac-148">JSON representation</span></span>
<span data-ttu-id="b03ac-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b03ac-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
