---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07a1dd94be6f73da420ba0cd3424030652eab2c5
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088200"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="92c8a-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="92c8a-103">deviceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="92c8a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92c8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92c8a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92c8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92c8a-106">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="92c8a-106">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="92c8a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92c8a-107">Properties</span></span>
|<span data-ttu-id="92c8a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92c8a-108">Property</span></span>|<span data-ttu-id="92c8a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="92c8a-109">Type</span></span>|<span data-ttu-id="92c8a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92c8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c8a-111">destino</span><span class="sxs-lookup"><span data-stu-id="92c8a-111">target</span></span>|[<span data-ttu-id="92c8a-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="92c8a-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="92c8a-113">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="92c8a-113">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92c8a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="92c8a-114">Relationships</span></span>
<span data-ttu-id="92c8a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92c8a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92c8a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92c8a-116">JSON Representation</span></span>
<span data-ttu-id="92c8a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92c8a-117">Here is a JSON representation of the resource.</span></span>
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



