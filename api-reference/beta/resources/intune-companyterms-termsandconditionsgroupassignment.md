---
title: tipo de recurso de termsAndConditionsGroupAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9ae49e1223c4b74fb8da8da7f5b42533fd33c8c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874214"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="71641-104">tipo de recurso de termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="71641-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71641-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71641-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71641-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71641-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71641-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71641-108">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma determinada termos e condições (T & C) política a um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="71641-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="71641-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="71641-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="71641-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="71641-110">Methods</span></span>
|<span data-ttu-id="71641-111">Método</span><span class="sxs-lookup"><span data-stu-id="71641-111">Method</span></span>|<span data-ttu-id="71641-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71641-112">Return Type</span></span>|<span data-ttu-id="71641-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="71641-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71641-114">Lista termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="71641-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="71641-115">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71641-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="71641-116">Lista as propriedades e os relacionamentos dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71641-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="71641-117">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="71641-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="71641-119">Leia as propriedades e os relacionamentos do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71641-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="71641-120">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="71641-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="71641-122">Crie um novo objeto de [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71641-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="71641-123">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="71641-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71641-124">None</span></span>|<span data-ttu-id="71641-125">Exclui um [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71641-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="71641-126">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="71641-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="71641-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="71641-128">Atualize as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71641-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71641-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71641-129">Properties</span></span>
|<span data-ttu-id="71641-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71641-130">Property</span></span>|<span data-ttu-id="71641-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71641-131">Type</span></span>|<span data-ttu-id="71641-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71641-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71641-133">id</span><span class="sxs-lookup"><span data-stu-id="71641-133">id</span></span>|<span data-ttu-id="71641-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71641-134">String</span></span>|<span data-ttu-id="71641-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="71641-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="71641-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="71641-136">targetGroupId</span></span>|<span data-ttu-id="71641-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71641-137">String</span></span>|<span data-ttu-id="71641-138">Identificador exclusivo de um grupo que a política de T & C é atribuída a.</span><span class="sxs-lookup"><span data-stu-id="71641-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71641-139">Relações</span><span class="sxs-lookup"><span data-stu-id="71641-139">Relationships</span></span>
|<span data-ttu-id="71641-140">Relação</span><span class="sxs-lookup"><span data-stu-id="71641-140">Relationship</span></span>|<span data-ttu-id="71641-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="71641-141">Type</span></span>|<span data-ttu-id="71641-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="71641-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71641-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="71641-143">termsAndConditions</span></span>|[<span data-ttu-id="71641-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="71641-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="71641-145">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="71641-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71641-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71641-146">JSON Representation</span></span>
<span data-ttu-id="71641-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71641-147">Here is a JSON representation of the resource.</span></span>
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





