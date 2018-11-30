---
title: tipo de recurso de termsAndConditionsGroupAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
ms.openlocfilehash: 071cd73ba36aaab74c7f5c36522c03014711286e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038747"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="43256-104">tipo de recurso de termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="43256-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43256-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43256-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43256-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43256-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43256-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43256-108">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma determinada termos e condições (T & C) política a um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="43256-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="43256-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="43256-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="43256-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="43256-110">Methods</span></span>
|<span data-ttu-id="43256-111">Método</span><span class="sxs-lookup"><span data-stu-id="43256-111">Method</span></span>|<span data-ttu-id="43256-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43256-112">Return Type</span></span>|<span data-ttu-id="43256-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="43256-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43256-114">Lista termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="43256-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="43256-115">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="43256-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="43256-116">Lista as propriedades e os relacionamentos dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="43256-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="43256-117">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="43256-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="43256-119">Leia as propriedades e os relacionamentos do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="43256-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="43256-120">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="43256-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="43256-122">Crie um novo objeto de [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="43256-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="43256-123">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="43256-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43256-124">None</span></span>|<span data-ttu-id="43256-125">Exclui um [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="43256-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="43256-126">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="43256-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="43256-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="43256-128">Atualize as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="43256-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43256-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43256-129">Properties</span></span>
|<span data-ttu-id="43256-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43256-130">Property</span></span>|<span data-ttu-id="43256-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43256-131">Type</span></span>|<span data-ttu-id="43256-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43256-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43256-133">id</span><span class="sxs-lookup"><span data-stu-id="43256-133">id</span></span>|<span data-ttu-id="43256-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43256-134">String</span></span>|<span data-ttu-id="43256-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="43256-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="43256-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="43256-136">targetGroupId</span></span>|<span data-ttu-id="43256-137">String</span><span class="sxs-lookup"><span data-stu-id="43256-137">String</span></span>|<span data-ttu-id="43256-138">Identificador exclusivo de um grupo que a política de T & C é atribuída a.</span><span class="sxs-lookup"><span data-stu-id="43256-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43256-139">Relações</span><span class="sxs-lookup"><span data-stu-id="43256-139">Relationships</span></span>
|<span data-ttu-id="43256-140">Relação</span><span class="sxs-lookup"><span data-stu-id="43256-140">Relationship</span></span>|<span data-ttu-id="43256-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="43256-141">Type</span></span>|<span data-ttu-id="43256-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="43256-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43256-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="43256-143">termsAndConditions</span></span>|[<span data-ttu-id="43256-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="43256-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="43256-145">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="43256-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43256-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43256-146">JSON Representation</span></span>
<span data-ttu-id="43256-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43256-147">Here is a JSON representation of the resource.</span></span>
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





