---
title: tipo de recurso windowsManagementAppHealthSummary
description: Contém propriedades para o resumo de integridade do aplicativo de gerenciamento do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07e782cb14ab2ee4996ff8e53f61323693e00846
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941685"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="dc12b-103">tipo de recurso windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="dc12b-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="dc12b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc12b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc12b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc12b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc12b-106">Contém propriedades para o resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="dc12b-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="dc12b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc12b-107">Methods</span></span>
|<span data-ttu-id="dc12b-108">Método</span><span class="sxs-lookup"><span data-stu-id="dc12b-108">Method</span></span>|<span data-ttu-id="dc12b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc12b-109">Return Type</span></span>|<span data-ttu-id="dc12b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc12b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc12b-111">Obter windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="dc12b-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="dc12b-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="dc12b-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="dc12b-113">Leia as propriedades e as relações do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="dc12b-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="dc12b-114">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="dc12b-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="dc12b-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="dc12b-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="dc12b-116">Atualiza as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="dc12b-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc12b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc12b-117">Properties</span></span>
|<span data-ttu-id="dc12b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc12b-118">Property</span></span>|<span data-ttu-id="dc12b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc12b-119">Type</span></span>|<span data-ttu-id="dc12b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc12b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc12b-121">id</span><span class="sxs-lookup"><span data-stu-id="dc12b-121">id</span></span>|<span data-ttu-id="dc12b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc12b-122">String</span></span>|<span data-ttu-id="dc12b-123">Chave da entidade de Resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="dc12b-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="dc12b-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc12b-124">healthyDeviceCount</span></span>|<span data-ttu-id="dc12b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="dc12b-125">Int32</span></span>|<span data-ttu-id="dc12b-126">Contagem de dispositivos íntegros.</span><span class="sxs-lookup"><span data-stu-id="dc12b-126">Healthy device count.</span></span>|
|<span data-ttu-id="dc12b-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc12b-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="dc12b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="dc12b-128">Int32</span></span>|<span data-ttu-id="dc12b-129">Contagem de dispositivos não íntegros.</span><span class="sxs-lookup"><span data-stu-id="dc12b-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="dc12b-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc12b-130">unknownDeviceCount</span></span>|<span data-ttu-id="dc12b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="dc12b-131">Int32</span></span>|<span data-ttu-id="dc12b-132">Contagem desconhecida de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dc12b-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc12b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="dc12b-133">Relationships</span></span>
<span data-ttu-id="dc12b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc12b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc12b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc12b-135">JSON Representation</span></span>
<span data-ttu-id="dc12b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc12b-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




