---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f4d0faada84b0c8436399f4ebd7b1e07392edd4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473855"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="7a64c-104">tipo de recurso termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-104">termsAndConditionsGroupAssignment resource type</span></span>

<span data-ttu-id="7a64c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a64c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a64c-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a64c-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a64c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a64c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a64c-108">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="7a64c-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="7a64c-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="7a64c-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="7a64c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a64c-110">Methods</span></span>
|<span data-ttu-id="7a64c-111">Método</span><span class="sxs-lookup"><span data-stu-id="7a64c-111">Method</span></span>|<span data-ttu-id="7a64c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a64c-112">Return Type</span></span>|<span data-ttu-id="7a64c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a64c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a64c-114">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="7a64c-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="7a64c-115">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a64c-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="7a64c-116">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7a64c-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="7a64c-117">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="7a64c-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7a64c-119">Leia as propriedades e as relações do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7a64c-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7a64c-120">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="7a64c-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7a64c-122">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7a64c-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7a64c-123">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="7a64c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a64c-124">None</span></span>|<span data-ttu-id="7a64c-125">Exclui [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7a64c-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="7a64c-126">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="7a64c-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a64c-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7a64c-128">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7a64c-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a64c-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a64c-129">Properties</span></span>
|<span data-ttu-id="7a64c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a64c-130">Property</span></span>|<span data-ttu-id="7a64c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a64c-131">Type</span></span>|<span data-ttu-id="7a64c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a64c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a64c-133">id</span><span class="sxs-lookup"><span data-stu-id="7a64c-133">id</span></span>|<span data-ttu-id="7a64c-134">String</span><span class="sxs-lookup"><span data-stu-id="7a64c-134">String</span></span>|<span data-ttu-id="7a64c-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="7a64c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7a64c-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7a64c-136">targetGroupId</span></span>|<span data-ttu-id="7a64c-137">String</span><span class="sxs-lookup"><span data-stu-id="7a64c-137">String</span></span>|<span data-ttu-id="7a64c-138">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="7a64c-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a64c-139">Relações</span><span class="sxs-lookup"><span data-stu-id="7a64c-139">Relationships</span></span>
|<span data-ttu-id="7a64c-140">Relação</span><span class="sxs-lookup"><span data-stu-id="7a64c-140">Relationship</span></span>|<span data-ttu-id="7a64c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a64c-141">Type</span></span>|<span data-ttu-id="7a64c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a64c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a64c-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="7a64c-143">termsAndConditions</span></span>|[<span data-ttu-id="7a64c-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="7a64c-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="7a64c-145">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="7a64c-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a64c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a64c-146">JSON Representation</span></span>
<span data-ttu-id="7a64c-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a64c-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```



