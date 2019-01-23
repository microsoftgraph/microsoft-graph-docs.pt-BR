---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2de08d2bc90061ed4096a9a010b332872eb36ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422023"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="cefc3-104">Tipo de recurso termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="cefc3-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cefc3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cefc3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cefc3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cefc3-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cefc3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefc3-108">Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo.</span><span class="sxs-lookup"><span data-stu-id="cefc3-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="cefc3-109">Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="cefc3-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="cefc3-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="cefc3-110">Methods</span></span>
|<span data-ttu-id="cefc3-111">Método</span><span class="sxs-lookup"><span data-stu-id="cefc3-111">Method</span></span>|<span data-ttu-id="cefc3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cefc3-112">Return Type</span></span>|<span data-ttu-id="cefc3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefc3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cefc3-114">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="cefc3-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="cefc3-115">Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cefc3-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="cefc3-116">Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cefc3-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="cefc3-117">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="cefc3-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="cefc3-119">Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cefc3-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="cefc3-120">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="cefc3-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="cefc3-122">Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cefc3-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="cefc3-123">Excluir termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="cefc3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cefc3-124">None</span></span>|<span data-ttu-id="cefc3-125">Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cefc3-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="cefc3-126">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="cefc3-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="cefc3-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="cefc3-128">Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cefc3-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cefc3-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cefc3-129">Properties</span></span>
|<span data-ttu-id="cefc3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cefc3-130">Property</span></span>|<span data-ttu-id="cefc3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefc3-131">Type</span></span>|<span data-ttu-id="cefc3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cefc3-133">id</span><span class="sxs-lookup"><span data-stu-id="cefc3-133">id</span></span>|<span data-ttu-id="cefc3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cefc3-134">String</span></span>|<span data-ttu-id="cefc3-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="cefc3-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="cefc3-136">destino</span><span class="sxs-lookup"><span data-stu-id="cefc3-136">target</span></span>|[<span data-ttu-id="cefc3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cefc3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cefc3-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="cefc3-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cefc3-139">Relações</span><span class="sxs-lookup"><span data-stu-id="cefc3-139">Relationships</span></span>
<span data-ttu-id="cefc3-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cefc3-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cefc3-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cefc3-141">JSON Representation</span></span>
<span data-ttu-id="cefc3-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cefc3-142">Here is a JSON representation of the resource.</span></span>
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




