---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b6bff777bfaf093d1148a584cc8524069304b70
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788481"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="32acc-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="32acc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32acc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32acc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32acc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32acc-107">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="32acc-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="32acc-108">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="32acc-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="32acc-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="32acc-109">Methods</span></span>
|<span data-ttu-id="32acc-110">Método</span><span class="sxs-lookup"><span data-stu-id="32acc-110">Method</span></span>|<span data-ttu-id="32acc-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32acc-111">Return Type</span></span>|<span data-ttu-id="32acc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="32acc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32acc-113">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="32acc-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="32acc-114">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32acc-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="32acc-115">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32acc-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="32acc-116">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="32acc-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="32acc-118">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32acc-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="32acc-119">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="32acc-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="32acc-121">Criar um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32acc-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="32acc-122">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="32acc-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32acc-123">None</span></span>|<span data-ttu-id="32acc-124">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32acc-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="32acc-125">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="32acc-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="32acc-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="32acc-127">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32acc-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32acc-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32acc-128">Properties</span></span>
|<span data-ttu-id="32acc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32acc-129">Property</span></span>|<span data-ttu-id="32acc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="32acc-130">Type</span></span>|<span data-ttu-id="32acc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="32acc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32acc-132">id</span><span class="sxs-lookup"><span data-stu-id="32acc-132">id</span></span>|<span data-ttu-id="32acc-133">String</span><span class="sxs-lookup"><span data-stu-id="32acc-133">String</span></span>|<span data-ttu-id="32acc-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="32acc-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="32acc-135">destino</span><span class="sxs-lookup"><span data-stu-id="32acc-135">target</span></span>|[<span data-ttu-id="32acc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="32acc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="32acc-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="32acc-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32acc-138">Relações</span><span class="sxs-lookup"><span data-stu-id="32acc-138">Relationships</span></span>
<span data-ttu-id="32acc-139">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="32acc-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32acc-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32acc-140">JSON Representation</span></span>
<span data-ttu-id="32acc-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32acc-141">Here is a JSON representation of the resource.</span></span>
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





