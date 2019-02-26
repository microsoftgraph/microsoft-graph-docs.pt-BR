---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5b97e691ff16ce2c86057ab5dae229d8657974
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142683"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="4c74e-104">tipo de recurso termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="4c74e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c74e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c74e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c74e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c74e-107">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="4c74e-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="4c74e-108">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="4c74e-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="4c74e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="4c74e-109">Methods</span></span>
|<span data-ttu-id="4c74e-110">Método</span><span class="sxs-lookup"><span data-stu-id="4c74e-110">Method</span></span>|<span data-ttu-id="4c74e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c74e-111">Return Type</span></span>|<span data-ttu-id="4c74e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c74e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c74e-113">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4c74e-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="4c74e-114">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4c74e-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="4c74e-115">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c74e-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="4c74e-116">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="4c74e-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4c74e-118">Leia as propriedades e as relações do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c74e-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4c74e-119">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="4c74e-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4c74e-121">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c74e-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4c74e-122">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="4c74e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c74e-123">None</span></span>|<span data-ttu-id="4c74e-124">Exclui [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c74e-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="4c74e-125">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="4c74e-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c74e-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4c74e-127">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c74e-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c74e-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c74e-128">Properties</span></span>
|<span data-ttu-id="4c74e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c74e-129">Property</span></span>|<span data-ttu-id="4c74e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c74e-130">Type</span></span>|<span data-ttu-id="4c74e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c74e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c74e-132">id</span><span class="sxs-lookup"><span data-stu-id="4c74e-132">id</span></span>|<span data-ttu-id="4c74e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c74e-133">String</span></span>|<span data-ttu-id="4c74e-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c74e-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4c74e-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4c74e-135">targetGroupId</span></span>|<span data-ttu-id="4c74e-136">String</span><span class="sxs-lookup"><span data-stu-id="4c74e-136">String</span></span>|<span data-ttu-id="4c74e-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="4c74e-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c74e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="4c74e-138">Relationships</span></span>
|<span data-ttu-id="4c74e-139">Relação</span><span class="sxs-lookup"><span data-stu-id="4c74e-139">Relationship</span></span>|<span data-ttu-id="4c74e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c74e-140">Type</span></span>|<span data-ttu-id="4c74e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c74e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c74e-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4c74e-142">termsAndConditions</span></span>|[<span data-ttu-id="4c74e-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4c74e-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="4c74e-144">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="4c74e-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c74e-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c74e-145">JSON Representation</span></span>
<span data-ttu-id="4c74e-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c74e-146">Here is a JSON representation of the resource.</span></span>
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




