---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e1caee5aebd46f6958077a9fea474327c629af0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273834"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="6ff6f-104">tipo de recurso termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-104">termsAndConditionsGroupAssignment resource type</span></span>

<span data-ttu-id="6ff6f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff6f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ff6f-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff6f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff6f-108">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="6ff6f-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="6ff6f-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6ff6f-110">Methods</span></span>
|<span data-ttu-id="6ff6f-111">Método</span><span class="sxs-lookup"><span data-stu-id="6ff6f-111">Method</span></span>|<span data-ttu-id="6ff6f-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6ff6f-112">Return Type</span></span>|<span data-ttu-id="6ff6f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff6f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ff6f-114">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="6ff6f-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="6ff6f-115">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6ff6f-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="6ff6f-116">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff6f-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="6ff6f-117">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="6ff6f-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6ff6f-119">Leia as propriedades e as relações do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff6f-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6ff6f-120">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="6ff6f-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6ff6f-122">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff6f-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6ff6f-123">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="6ff6f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ff6f-124">None</span></span>|<span data-ttu-id="6ff6f-125">Exclui [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ff6f-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="6ff6f-126">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="6ff6f-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6ff6f-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6ff6f-128">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff6f-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ff6f-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ff6f-129">Properties</span></span>
|<span data-ttu-id="6ff6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ff6f-130">Property</span></span>|<span data-ttu-id="6ff6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff6f-131">Type</span></span>|<span data-ttu-id="6ff6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff6f-133">id</span><span class="sxs-lookup"><span data-stu-id="6ff6f-133">id</span></span>|<span data-ttu-id="6ff6f-134">String</span><span class="sxs-lookup"><span data-stu-id="6ff6f-134">String</span></span>|<span data-ttu-id="6ff6f-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6ff6f-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="6ff6f-136">targetGroupId</span></span>|<span data-ttu-id="6ff6f-137">String</span><span class="sxs-lookup"><span data-stu-id="6ff6f-137">String</span></span>|<span data-ttu-id="6ff6f-138">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff6f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6ff6f-139">Relationships</span></span>
|<span data-ttu-id="6ff6f-140">Relação</span><span class="sxs-lookup"><span data-stu-id="6ff6f-140">Relationship</span></span>|<span data-ttu-id="6ff6f-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff6f-141">Type</span></span>|<span data-ttu-id="6ff6f-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff6f-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff6f-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6ff6f-143">termsAndConditions</span></span>|[<span data-ttu-id="6ff6f-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6ff6f-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="6ff6f-145">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ff6f-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ff6f-146">JSON Representation</span></span>
<span data-ttu-id="6ff6f-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ff6f-147">Here is a JSON representation of the resource.</span></span>
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




