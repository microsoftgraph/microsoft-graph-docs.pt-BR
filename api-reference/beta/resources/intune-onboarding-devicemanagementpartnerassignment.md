---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 306acfae948a81ca5c8933f455a21347bf27ee9e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778719"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="c33fd-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="c33fd-103">deviceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="c33fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c33fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c33fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c33fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33fd-106">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c33fd-106">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="c33fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c33fd-107">Properties</span></span>
|<span data-ttu-id="c33fd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c33fd-108">Property</span></span>|<span data-ttu-id="c33fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33fd-109">Type</span></span>|<span data-ttu-id="c33fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33fd-111">destino</span><span class="sxs-lookup"><span data-stu-id="c33fd-111">target</span></span>|[<span data-ttu-id="c33fd-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c33fd-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c33fd-113">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c33fd-113">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c33fd-114">Relações</span><span class="sxs-lookup"><span data-stu-id="c33fd-114">Relationships</span></span>
<span data-ttu-id="c33fd-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c33fd-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c33fd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c33fd-116">JSON Representation</span></span>
<span data-ttu-id="c33fd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c33fd-117">Here is a JSON representation of the resource.</span></span>
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



