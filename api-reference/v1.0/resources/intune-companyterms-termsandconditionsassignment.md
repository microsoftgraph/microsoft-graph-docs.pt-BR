---
title: Tipo de recurso termsAndConditionsAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
ms.openlocfilehash: 848998e59f214fc679aba7c27a2a529be05c8adc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006211"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="5baf2-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="5baf2-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5baf2-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5baf2-106">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="5baf2-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="5baf2-107">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="5baf2-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="5baf2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5baf2-108">Methods</span></span>
|<span data-ttu-id="5baf2-109">Método</span><span class="sxs-lookup"><span data-stu-id="5baf2-109">Method</span></span>|<span data-ttu-id="5baf2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5baf2-110">Return Type</span></span>|<span data-ttu-id="5baf2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5baf2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5baf2-112">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="5baf2-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="5baf2-113">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5baf2-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="5baf2-114">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5baf2-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="5baf2-115">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="5baf2-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5baf2-117">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5baf2-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="5baf2-118">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="5baf2-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5baf2-120">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5baf2-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="5baf2-121">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="5baf2-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5baf2-122">None</span></span>|<span data-ttu-id="5baf2-123">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5baf2-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="5baf2-124">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="5baf2-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5baf2-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5baf2-126">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5baf2-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5baf2-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5baf2-127">Properties</span></span>
|<span data-ttu-id="5baf2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5baf2-128">Property</span></span>|<span data-ttu-id="5baf2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5baf2-129">Type</span></span>|<span data-ttu-id="5baf2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5baf2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5baf2-131">id</span><span class="sxs-lookup"><span data-stu-id="5baf2-131">id</span></span>|<span data-ttu-id="5baf2-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5baf2-132">String</span></span>|<span data-ttu-id="5baf2-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="5baf2-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5baf2-134">destino</span><span class="sxs-lookup"><span data-stu-id="5baf2-134">target</span></span>|[<span data-ttu-id="5baf2-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5baf2-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5baf2-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="5baf2-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5baf2-137">Relações</span><span class="sxs-lookup"><span data-stu-id="5baf2-137">Relationships</span></span>
<span data-ttu-id="5baf2-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5baf2-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5baf2-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5baf2-139">JSON Representation</span></span>
<span data-ttu-id="5baf2-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5baf2-140">Here is a JSON representation of the resource.</span></span>
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



