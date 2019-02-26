---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e4c8b7ac86f86f2b89bcd21a0576f68b823b9f6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262199"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="91d12-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="91d12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91d12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91d12-106">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="91d12-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="91d12-107">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="91d12-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="91d12-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="91d12-108">Methods</span></span>
|<span data-ttu-id="91d12-109">Método</span><span class="sxs-lookup"><span data-stu-id="91d12-109">Method</span></span>|<span data-ttu-id="91d12-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="91d12-110">Return Type</span></span>|<span data-ttu-id="91d12-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="91d12-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91d12-112">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="91d12-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="91d12-113">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="91d12-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="91d12-114">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91d12-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="91d12-115">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="91d12-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="91d12-117">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91d12-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="91d12-118">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="91d12-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="91d12-120">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91d12-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="91d12-121">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="91d12-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91d12-122">None</span></span>|<span data-ttu-id="91d12-123">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91d12-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="91d12-124">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="91d12-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="91d12-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="91d12-126">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91d12-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="91d12-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91d12-127">Properties</span></span>
|<span data-ttu-id="91d12-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91d12-128">Property</span></span>|<span data-ttu-id="91d12-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="91d12-129">Type</span></span>|<span data-ttu-id="91d12-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="91d12-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91d12-131">id</span><span class="sxs-lookup"><span data-stu-id="91d12-131">id</span></span>|<span data-ttu-id="91d12-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91d12-132">String</span></span>|<span data-ttu-id="91d12-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="91d12-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="91d12-134">destino</span><span class="sxs-lookup"><span data-stu-id="91d12-134">target</span></span>|[<span data-ttu-id="91d12-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="91d12-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="91d12-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="91d12-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91d12-137">Relações</span><span class="sxs-lookup"><span data-stu-id="91d12-137">Relationships</span></span>
<span data-ttu-id="91d12-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="91d12-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91d12-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91d12-139">JSON Representation</span></span>
<span data-ttu-id="91d12-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91d12-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



