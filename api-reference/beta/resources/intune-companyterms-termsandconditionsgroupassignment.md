---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f3518dcc31bf703d3fe42e6bab15d5731d5beb5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800914"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="3a454-104">tipo de recurso termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="3a454-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a454-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a454-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a454-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a454-107">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="3a454-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="3a454-108">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="3a454-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="3a454-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a454-109">Methods</span></span>
|<span data-ttu-id="3a454-110">Método</span><span class="sxs-lookup"><span data-stu-id="3a454-110">Method</span></span>|<span data-ttu-id="3a454-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3a454-111">Return Type</span></span>|<span data-ttu-id="3a454-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a454-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a454-113">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3a454-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="3a454-114">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3a454-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="3a454-115">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3a454-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="3a454-116">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="3a454-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3a454-118">Leia as propriedades e as relações do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3a454-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3a454-119">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="3a454-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3a454-121">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3a454-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3a454-122">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="3a454-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a454-123">None</span></span>|<span data-ttu-id="3a454-124">Exclui [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3a454-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="3a454-125">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="3a454-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3a454-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3a454-127">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3a454-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a454-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a454-128">Properties</span></span>
|<span data-ttu-id="3a454-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a454-129">Property</span></span>|<span data-ttu-id="3a454-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a454-130">Type</span></span>|<span data-ttu-id="3a454-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a454-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a454-132">id</span><span class="sxs-lookup"><span data-stu-id="3a454-132">id</span></span>|<span data-ttu-id="3a454-133">String</span><span class="sxs-lookup"><span data-stu-id="3a454-133">String</span></span>|<span data-ttu-id="3a454-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="3a454-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3a454-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3a454-135">targetGroupId</span></span>|<span data-ttu-id="3a454-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a454-136">String</span></span>|<span data-ttu-id="3a454-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="3a454-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a454-138">Relações</span><span class="sxs-lookup"><span data-stu-id="3a454-138">Relationships</span></span>
|<span data-ttu-id="3a454-139">Relação</span><span class="sxs-lookup"><span data-stu-id="3a454-139">Relationship</span></span>|<span data-ttu-id="3a454-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a454-140">Type</span></span>|<span data-ttu-id="3a454-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a454-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a454-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3a454-142">termsAndConditions</span></span>|[<span data-ttu-id="3a454-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3a454-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="3a454-144">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="3a454-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a454-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a454-145">JSON Representation</span></span>
<span data-ttu-id="3a454-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a454-146">Here is a JSON representation of the resource.</span></span>
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





