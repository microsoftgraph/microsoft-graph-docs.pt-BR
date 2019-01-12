---
title: Tipo de recurso termsAndConditionsAssignment
description: C) política a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75c9946cead03b2d7c0630c29a9b28c47ac1b269
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919802"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="ea08f-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="ea08f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea08f-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea08f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea08f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea08f-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea08f-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea08f-108">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="ea08f-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="ea08f-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="ea08f-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="ea08f-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea08f-110">Methods</span></span>
|<span data-ttu-id="ea08f-111">Método</span><span class="sxs-lookup"><span data-stu-id="ea08f-111">Method</span></span>|<span data-ttu-id="ea08f-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea08f-112">Return Type</span></span>|<span data-ttu-id="ea08f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea08f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea08f-114">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="ea08f-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="ea08f-115">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea08f-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="ea08f-116">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea08f-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="ea08f-117">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="ea08f-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ea08f-119">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea08f-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="ea08f-120">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="ea08f-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ea08f-122">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea08f-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="ea08f-123">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="ea08f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea08f-124">None</span></span>|<span data-ttu-id="ea08f-125">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea08f-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="ea08f-126">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="ea08f-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ea08f-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ea08f-128">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea08f-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea08f-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea08f-129">Properties</span></span>
|<span data-ttu-id="ea08f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea08f-130">Property</span></span>|<span data-ttu-id="ea08f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea08f-131">Type</span></span>|<span data-ttu-id="ea08f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea08f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea08f-133">id</span><span class="sxs-lookup"><span data-stu-id="ea08f-133">id</span></span>|<span data-ttu-id="ea08f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea08f-134">String</span></span>|<span data-ttu-id="ea08f-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea08f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ea08f-136">destino</span><span class="sxs-lookup"><span data-stu-id="ea08f-136">target</span></span>|[<span data-ttu-id="ea08f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ea08f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ea08f-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="ea08f-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea08f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ea08f-139">Relationships</span></span>
<span data-ttu-id="ea08f-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea08f-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea08f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea08f-141">JSON Representation</span></span>
<span data-ttu-id="ea08f-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea08f-142">Here is a JSON representation of the resource.</span></span>
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





