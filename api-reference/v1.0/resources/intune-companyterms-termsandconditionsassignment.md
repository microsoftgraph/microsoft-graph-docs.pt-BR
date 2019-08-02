---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b11f96cb6c8b1062c25e194ab8e3d96ea7c1deeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031980"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="0577e-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="0577e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0577e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0577e-106">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="0577e-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="0577e-107">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="0577e-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="0577e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0577e-108">Methods</span></span>
|<span data-ttu-id="0577e-109">Método</span><span class="sxs-lookup"><span data-stu-id="0577e-109">Method</span></span>|<span data-ttu-id="0577e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0577e-110">Return Type</span></span>|<span data-ttu-id="0577e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0577e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0577e-112">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="0577e-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="0577e-113">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0577e-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="0577e-114">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0577e-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="0577e-115">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="0577e-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="0577e-117">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0577e-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="0577e-118">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="0577e-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="0577e-120">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0577e-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="0577e-121">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="0577e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0577e-122">None</span></span>|<span data-ttu-id="0577e-123">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0577e-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="0577e-124">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="0577e-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0577e-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="0577e-126">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0577e-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0577e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0577e-127">Properties</span></span>
|<span data-ttu-id="0577e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0577e-128">Property</span></span>|<span data-ttu-id="0577e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0577e-129">Type</span></span>|<span data-ttu-id="0577e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0577e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0577e-131">id</span><span class="sxs-lookup"><span data-stu-id="0577e-131">id</span></span>|<span data-ttu-id="0577e-132">String</span><span class="sxs-lookup"><span data-stu-id="0577e-132">String</span></span>|<span data-ttu-id="0577e-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="0577e-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0577e-134">destino</span><span class="sxs-lookup"><span data-stu-id="0577e-134">target</span></span>|[<span data-ttu-id="0577e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0577e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0577e-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="0577e-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0577e-137">Relações</span><span class="sxs-lookup"><span data-stu-id="0577e-137">Relationships</span></span>
<span data-ttu-id="0577e-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0577e-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0577e-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0577e-139">JSON Representation</span></span>
<span data-ttu-id="0577e-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0577e-140">Here is a JSON representation of the resource.</span></span>
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



