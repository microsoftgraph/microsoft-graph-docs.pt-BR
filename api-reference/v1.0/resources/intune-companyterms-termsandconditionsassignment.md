---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead01aac6a0ae8b297b6c013ce2a2a3b4e421956
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758922"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="a7c5f-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="a7c5f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c5f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7c5f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c5f-107">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="a7c5f-108">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="a7c5f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a7c5f-109">Methods</span></span>
|<span data-ttu-id="a7c5f-110">Método</span><span class="sxs-lookup"><span data-stu-id="a7c5f-110">Method</span></span>|<span data-ttu-id="a7c5f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a7c5f-111">Return Type</span></span>|<span data-ttu-id="a7c5f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c5f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7c5f-113">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="a7c5f-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="a7c5f-114">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7c5f-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="a7c5f-115">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7c5f-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="a7c5f-116">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="a7c5f-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a7c5f-118">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7c5f-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="a7c5f-119">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="a7c5f-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a7c5f-121">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7c5f-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="a7c5f-122">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="a7c5f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7c5f-123">None</span></span>|<span data-ttu-id="a7c5f-124">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7c5f-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="a7c5f-125">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="a7c5f-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c5f-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a7c5f-127">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7c5f-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7c5f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c5f-128">Properties</span></span>
|<span data-ttu-id="a7c5f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c5f-129">Property</span></span>|<span data-ttu-id="a7c5f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c5f-130">Type</span></span>|<span data-ttu-id="a7c5f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c5f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c5f-132">id</span><span class="sxs-lookup"><span data-stu-id="a7c5f-132">id</span></span>|<span data-ttu-id="a7c5f-133">String</span><span class="sxs-lookup"><span data-stu-id="a7c5f-133">String</span></span>|<span data-ttu-id="a7c5f-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a7c5f-135">destino</span><span class="sxs-lookup"><span data-stu-id="a7c5f-135">target</span></span>|[<span data-ttu-id="a7c5f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a7c5f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a7c5f-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c5f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a7c5f-138">Relationships</span></span>
<span data-ttu-id="a7c5f-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7c5f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7c5f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c5f-140">JSON Representation</span></span>
<span data-ttu-id="a7c5f-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c5f-141">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




