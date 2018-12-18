---
title: Tipo de recurso termsAndConditionsAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
ms.openlocfilehash: cfc38c491cc7c619dd6e3fea42fc2b1f34b20847
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311995"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="816d1-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="816d1-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="816d1-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="816d1-106">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="816d1-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="816d1-107">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="816d1-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="816d1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="816d1-108">Methods</span></span>
|<span data-ttu-id="816d1-109">Método</span><span class="sxs-lookup"><span data-stu-id="816d1-109">Method</span></span>|<span data-ttu-id="816d1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="816d1-110">Return Type</span></span>|<span data-ttu-id="816d1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="816d1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="816d1-112">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="816d1-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="816d1-113">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="816d1-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="816d1-114">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="816d1-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="816d1-115">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="816d1-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="816d1-117">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="816d1-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="816d1-118">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="816d1-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="816d1-120">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="816d1-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="816d1-121">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="816d1-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="816d1-122">None</span></span>|<span data-ttu-id="816d1-123">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="816d1-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="816d1-124">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="816d1-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="816d1-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="816d1-126">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="816d1-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="816d1-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="816d1-127">Properties</span></span>
|<span data-ttu-id="816d1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="816d1-128">Property</span></span>|<span data-ttu-id="816d1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="816d1-129">Type</span></span>|<span data-ttu-id="816d1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="816d1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="816d1-131">id</span><span class="sxs-lookup"><span data-stu-id="816d1-131">id</span></span>|<span data-ttu-id="816d1-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="816d1-132">String</span></span>|<span data-ttu-id="816d1-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="816d1-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="816d1-134">destino</span><span class="sxs-lookup"><span data-stu-id="816d1-134">target</span></span>|[<span data-ttu-id="816d1-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="816d1-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="816d1-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="816d1-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="816d1-137">Relações</span><span class="sxs-lookup"><span data-stu-id="816d1-137">Relationships</span></span>
<span data-ttu-id="816d1-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="816d1-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="816d1-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="816d1-139">JSON Representation</span></span>
<span data-ttu-id="816d1-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="816d1-140">Here is a JSON representation of the resource.</span></span>
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



