---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb74dad5b75202d908b82b87e7fd66f7447aa826
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154912"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="b96fc-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="b96fc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96fc-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b96fc-106">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b96fc-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b96fc-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b96fc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b96fc-108">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="b96fc-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="b96fc-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="b96fc-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="b96fc-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="b96fc-110">Methods</span></span>
|<span data-ttu-id="b96fc-111">Método</span><span class="sxs-lookup"><span data-stu-id="b96fc-111">Method</span></span>|<span data-ttu-id="b96fc-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b96fc-112">Return Type</span></span>|<span data-ttu-id="b96fc-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96fc-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b96fc-114">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="b96fc-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="b96fc-115">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b96fc-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="b96fc-116">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b96fc-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="b96fc-117">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="b96fc-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b96fc-119">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b96fc-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="b96fc-120">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="b96fc-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b96fc-122">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b96fc-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="b96fc-123">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="b96fc-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b96fc-124">None</span></span>|<span data-ttu-id="b96fc-125">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b96fc-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="b96fc-126">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="b96fc-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b96fc-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b96fc-128">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b96fc-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b96fc-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b96fc-129">Properties</span></span>
|<span data-ttu-id="b96fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b96fc-130">Property</span></span>|<span data-ttu-id="b96fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b96fc-131">Type</span></span>|<span data-ttu-id="b96fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96fc-133">id</span><span class="sxs-lookup"><span data-stu-id="b96fc-133">id</span></span>|<span data-ttu-id="b96fc-134">String</span><span class="sxs-lookup"><span data-stu-id="b96fc-134">String</span></span>|<span data-ttu-id="b96fc-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="b96fc-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b96fc-136">destino</span><span class="sxs-lookup"><span data-stu-id="b96fc-136">target</span></span>|[<span data-ttu-id="b96fc-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b96fc-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b96fc-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="b96fc-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b96fc-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b96fc-139">Relationships</span></span>
<span data-ttu-id="b96fc-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b96fc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b96fc-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b96fc-141">JSON Representation</span></span>
<span data-ttu-id="b96fc-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b96fc-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




