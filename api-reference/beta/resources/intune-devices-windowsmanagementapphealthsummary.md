---
title: tipo de recurso windowsManagementAppHealthSummary
description: Contém propriedades para o resumo de integridade do aplicativo de gerenciamento do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8033f5e66928de4e0f913eaaab0aaa271fa2894
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983976"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="a800e-103">tipo de recurso windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="a800e-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="a800e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a800e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a800e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a800e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a800e-106">Contém propriedades para o resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="a800e-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="a800e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a800e-107">Methods</span></span>
|<span data-ttu-id="a800e-108">Método</span><span class="sxs-lookup"><span data-stu-id="a800e-108">Method</span></span>|<span data-ttu-id="a800e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a800e-109">Return Type</span></span>|<span data-ttu-id="a800e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a800e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a800e-111">Obter windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="a800e-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="a800e-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="a800e-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="a800e-113">Leia as propriedades e as relações do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a800e-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="a800e-114">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="a800e-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="a800e-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="a800e-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="a800e-116">Atualiza as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a800e-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a800e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a800e-117">Properties</span></span>
|<span data-ttu-id="a800e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a800e-118">Property</span></span>|<span data-ttu-id="a800e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a800e-119">Type</span></span>|<span data-ttu-id="a800e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a800e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a800e-121">id</span><span class="sxs-lookup"><span data-stu-id="a800e-121">id</span></span>|<span data-ttu-id="a800e-122">String</span><span class="sxs-lookup"><span data-stu-id="a800e-122">String</span></span>|<span data-ttu-id="a800e-123">Chave da entidade de Resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="a800e-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="a800e-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a800e-124">healthyDeviceCount</span></span>|<span data-ttu-id="a800e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a800e-125">Int32</span></span>|<span data-ttu-id="a800e-126">Contagem de dispositivos íntegros.</span><span class="sxs-lookup"><span data-stu-id="a800e-126">Healthy device count.</span></span>|
|<span data-ttu-id="a800e-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a800e-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="a800e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a800e-128">Int32</span></span>|<span data-ttu-id="a800e-129">Contagem de dispositivos não íntegros.</span><span class="sxs-lookup"><span data-stu-id="a800e-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="a800e-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a800e-130">unknownDeviceCount</span></span>|<span data-ttu-id="a800e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a800e-131">Int32</span></span>|<span data-ttu-id="a800e-132">Contagem desconhecida de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a800e-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a800e-133">Relações</span><span class="sxs-lookup"><span data-stu-id="a800e-133">Relationships</span></span>
<span data-ttu-id="a800e-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a800e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a800e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a800e-135">JSON Representation</span></span>
<span data-ttu-id="a800e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a800e-136">Here is a JSON representation of the resource.</span></span>
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





