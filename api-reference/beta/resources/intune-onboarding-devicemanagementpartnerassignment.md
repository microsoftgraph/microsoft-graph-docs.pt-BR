---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ae96c45002e4006917f0cfa2a1aff207b1ea71f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178798"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="395e7-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="395e7-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="395e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="395e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="395e7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="395e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="395e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="395e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="395e7-107">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="395e7-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="395e7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="395e7-108">Properties</span></span>
|<span data-ttu-id="395e7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="395e7-109">Property</span></span>|<span data-ttu-id="395e7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="395e7-110">Type</span></span>|<span data-ttu-id="395e7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="395e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="395e7-112">destino</span><span class="sxs-lookup"><span data-stu-id="395e7-112">target</span></span>|[<span data-ttu-id="395e7-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="395e7-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="395e7-114">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="395e7-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="395e7-115">Relações</span><span class="sxs-lookup"><span data-stu-id="395e7-115">Relationships</span></span>
<span data-ttu-id="395e7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="395e7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="395e7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="395e7-117">JSON Representation</span></span>
<span data-ttu-id="395e7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="395e7-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



