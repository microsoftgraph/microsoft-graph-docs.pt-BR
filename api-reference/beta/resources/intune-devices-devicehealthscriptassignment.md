---
title: tipo de recurso deviceHealthScriptAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a37d36fd5b36384d62ef656b9d36a7ed870e3586
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539089"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="6a28d-103">tipo de recurso deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6a28d-103">deviceHealthScriptAssignment resource type</span></span>

> <span data-ttu-id="6a28d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a28d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a28d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a28d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a28d-106">Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.</span><span class="sxs-lookup"><span data-stu-id="6a28d-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="6a28d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a28d-107">Methods</span></span>
|<span data-ttu-id="6a28d-108">Método</span><span class="sxs-lookup"><span data-stu-id="6a28d-108">Method</span></span>|<span data-ttu-id="6a28d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a28d-109">Return Type</span></span>|<span data-ttu-id="6a28d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a28d-110">Description</span></span>|
|:---|:---|:---|
<span data-ttu-id="6a28d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a28d-111">None</span></span>

## <a name="properties"></a><span data-ttu-id="6a28d-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a28d-112">Properties</span></span>
|<span data-ttu-id="6a28d-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a28d-113">Property</span></span>|<span data-ttu-id="6a28d-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a28d-114">Type</span></span>|<span data-ttu-id="6a28d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a28d-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a28d-116">id</span><span class="sxs-lookup"><span data-stu-id="6a28d-116">id</span></span>|<span data-ttu-id="6a28d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a28d-117">String</span></span>|<span data-ttu-id="6a28d-118">Chave da entidade de atribuição de script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6a28d-118">Key of the device health script assignment entity</span></span>|
|<span data-ttu-id="6a28d-119">destino</span><span class="sxs-lookup"><span data-stu-id="6a28d-119">target</span></span>|[<span data-ttu-id="6a28d-120">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6a28d-120">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6a28d-121">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="6a28d-121">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="6a28d-122">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="6a28d-122">runRemediationScript</span></span>|<span data-ttu-id="6a28d-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a28d-123">Boolean</span></span>|<span data-ttu-id="6a28d-124">Determinar se queremos executar somente o script de detecção ou executar o script de detecção e o script de correção</span><span class="sxs-lookup"><span data-stu-id="6a28d-124">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="6a28d-125">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6a28d-125">runSchedule</span></span>|[<span data-ttu-id="6a28d-126">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6a28d-126">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="6a28d-127">O grupo do Azure Active Directory que estamos direcionando o script para</span><span class="sxs-lookup"><span data-stu-id="6a28d-127">The Azure Active Directory group we are targeting the script to</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a28d-128">Relações</span><span class="sxs-lookup"><span data-stu-id="6a28d-128">Relationships</span></span>
<span data-ttu-id="6a28d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a28d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a28d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a28d-130">JSON Representation</span></span>
<span data-ttu-id="6a28d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a28d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



