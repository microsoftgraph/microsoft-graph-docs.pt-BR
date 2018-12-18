---
title: Tipo de recurso termsAndConditionsAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
ms.openlocfilehash: a7b0e9deb391b9431be1ed4f282cb6e5a63ced6e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351048"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="7495e-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="7495e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7495e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7495e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7495e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7495e-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7495e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7495e-108">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="7495e-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="7495e-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="7495e-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="7495e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7495e-110">Methods</span></span>
|<span data-ttu-id="7495e-111">Método</span><span class="sxs-lookup"><span data-stu-id="7495e-111">Method</span></span>|<span data-ttu-id="7495e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7495e-112">Return Type</span></span>|<span data-ttu-id="7495e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7495e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7495e-114">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="7495e-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="7495e-115">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7495e-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="7495e-116">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7495e-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="7495e-117">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="7495e-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7495e-119">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7495e-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7495e-120">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="7495e-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7495e-122">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7495e-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7495e-123">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="7495e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7495e-124">None</span></span>|<span data-ttu-id="7495e-125">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7495e-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="7495e-126">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="7495e-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7495e-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7495e-128">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7495e-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7495e-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7495e-129">Properties</span></span>
|<span data-ttu-id="7495e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7495e-130">Property</span></span>|<span data-ttu-id="7495e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7495e-131">Type</span></span>|<span data-ttu-id="7495e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7495e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7495e-133">id</span><span class="sxs-lookup"><span data-stu-id="7495e-133">id</span></span>|<span data-ttu-id="7495e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7495e-134">String</span></span>|<span data-ttu-id="7495e-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="7495e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7495e-136">destino</span><span class="sxs-lookup"><span data-stu-id="7495e-136">target</span></span>|[<span data-ttu-id="7495e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7495e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7495e-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="7495e-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7495e-139">Relações</span><span class="sxs-lookup"><span data-stu-id="7495e-139">Relationships</span></span>
<span data-ttu-id="7495e-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7495e-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7495e-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7495e-141">JSON Representation</span></span>
<span data-ttu-id="7495e-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7495e-142">Here is a JSON representation of the resource.</span></span>
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





