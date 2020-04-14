---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bee2745c7757ed31d18c3a05916b1e9aa0bec41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455648"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="d837d-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="d837d-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="d837d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d837d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d837d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d837d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d837d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d837d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d837d-107">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d837d-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="d837d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d837d-108">Properties</span></span>
|<span data-ttu-id="d837d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d837d-109">Property</span></span>|<span data-ttu-id="d837d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d837d-110">Type</span></span>|<span data-ttu-id="d837d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d837d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d837d-112">destino</span><span class="sxs-lookup"><span data-stu-id="d837d-112">target</span></span>|[<span data-ttu-id="d837d-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d837d-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d837d-114">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d837d-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d837d-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d837d-115">Relationships</span></span>
<span data-ttu-id="d837d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d837d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d837d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d837d-117">JSON Representation</span></span>
<span data-ttu-id="d837d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d837d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



