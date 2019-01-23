---
title: tipo de recurso de termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de um dado termos e condições (T&C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418572"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="efb17-104">tipo de recurso de termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="efb17-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="efb17-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="efb17-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efb17-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efb17-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="efb17-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb17-108">Uma entidade termsAndConditionsGroupAssignment representa a atribuição de um dado termos e condições (T&C) política a um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="efb17-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="efb17-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="efb17-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="efb17-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="efb17-110">Methods</span></span>
|<span data-ttu-id="efb17-111">Método</span><span class="sxs-lookup"><span data-stu-id="efb17-111">Method</span></span>|<span data-ttu-id="efb17-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="efb17-112">Return Type</span></span>|<span data-ttu-id="efb17-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb17-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efb17-114">Lista termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="efb17-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="efb17-115">coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="efb17-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="efb17-116">Lista as propriedades e os relacionamentos dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="efb17-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="efb17-117">Obter termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="efb17-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efb17-119">Leia as propriedades e os relacionamentos do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="efb17-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="efb17-120">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="efb17-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efb17-122">Crie um novo objeto de [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="efb17-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="efb17-123">Excluir termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="efb17-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efb17-124">None</span></span>|<span data-ttu-id="efb17-125">Exclui um [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efb17-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="efb17-126">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="efb17-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efb17-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efb17-128">Atualize as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="efb17-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="efb17-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efb17-129">Properties</span></span>
|<span data-ttu-id="efb17-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efb17-130">Property</span></span>|<span data-ttu-id="efb17-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb17-131">Type</span></span>|<span data-ttu-id="efb17-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb17-133">id</span><span class="sxs-lookup"><span data-stu-id="efb17-133">id</span></span>|<span data-ttu-id="efb17-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efb17-134">String</span></span>|<span data-ttu-id="efb17-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="efb17-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="efb17-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="efb17-136">targetGroupId</span></span>|<span data-ttu-id="efb17-137">String</span><span class="sxs-lookup"><span data-stu-id="efb17-137">String</span></span>|<span data-ttu-id="efb17-138">Identificador exclusivo de um grupo que a política de T&C é atribuída a.</span><span class="sxs-lookup"><span data-stu-id="efb17-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efb17-139">Relações</span><span class="sxs-lookup"><span data-stu-id="efb17-139">Relationships</span></span>
|<span data-ttu-id="efb17-140">Relação</span><span class="sxs-lookup"><span data-stu-id="efb17-140">Relationship</span></span>|<span data-ttu-id="efb17-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb17-141">Type</span></span>|<span data-ttu-id="efb17-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb17-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb17-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="efb17-143">termsAndConditions</span></span>|[<span data-ttu-id="efb17-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="efb17-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="efb17-145">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="efb17-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efb17-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efb17-146">JSON Representation</span></span>
<span data-ttu-id="efb17-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efb17-147">Here is a JSON representation of the resource.</span></span>
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




