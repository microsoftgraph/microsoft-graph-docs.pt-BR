---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5427be3bd28b46d18e4342e1731255c2675d910
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524115"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="a4f9c-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="a4f9c-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="a4f9c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4f9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4f9c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4f9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4f9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4f9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4f9c-107">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a4f9c-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="a4f9c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4f9c-108">Properties</span></span>
|<span data-ttu-id="a4f9c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4f9c-109">Property</span></span>|<span data-ttu-id="a4f9c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4f9c-110">Type</span></span>|<span data-ttu-id="a4f9c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4f9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4f9c-112">destino</span><span class="sxs-lookup"><span data-stu-id="a4f9c-112">target</span></span>|[<span data-ttu-id="a4f9c-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a4f9c-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a4f9c-114">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="a4f9c-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4f9c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a4f9c-115">Relationships</span></span>
<span data-ttu-id="a4f9c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4f9c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4f9c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4f9c-117">JSON Representation</span></span>
<span data-ttu-id="a4f9c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4f9c-118">Here is a JSON representation of the resource.</span></span>
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



