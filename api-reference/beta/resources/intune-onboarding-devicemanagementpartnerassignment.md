---
title: Tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Dispositivos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0cda49b654313ec4d69e810033ae681b8ac2645
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157537"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="fc56b-103">Tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="fc56b-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="fc56b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc56b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc56b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc56b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc56b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc56b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc56b-107">Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Dispositivos</span><span class="sxs-lookup"><span data-stu-id="fc56b-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="fc56b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc56b-108">Properties</span></span>
|<span data-ttu-id="fc56b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc56b-109">Property</span></span>|<span data-ttu-id="fc56b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc56b-110">Type</span></span>|<span data-ttu-id="fc56b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc56b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc56b-112">destino</span><span class="sxs-lookup"><span data-stu-id="fc56b-112">target</span></span>|[<span data-ttu-id="fc56b-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fc56b-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fc56b-114">Grupos de usuários voltados para dispositivos a serem inscritos por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="fc56b-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc56b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="fc56b-115">Relationships</span></span>
<span data-ttu-id="fc56b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc56b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc56b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc56b-117">JSON Representation</span></span>
<span data-ttu-id="fc56b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc56b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




