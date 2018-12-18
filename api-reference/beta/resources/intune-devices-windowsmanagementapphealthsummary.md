---
title: tipo de recurso de windowsManagementAppHealthSummary
description: Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.
author: tfitzmac
ms.openlocfilehash: 5717f96cbac534f2726ccf7bcfcbdb54d4c17b28
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326226"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="d4bc3-103">tipo de recurso de windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="d4bc3-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="d4bc3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4bc3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4bc3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4bc3-107">Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="d4bc3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4bc3-108">Methods</span></span>
|<span data-ttu-id="d4bc3-109">Método</span><span class="sxs-lookup"><span data-stu-id="d4bc3-109">Method</span></span>|<span data-ttu-id="d4bc3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4bc3-110">Return Type</span></span>|<span data-ttu-id="d4bc3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4bc3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4bc3-112">Obter windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="d4bc3-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="d4bc3-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="d4bc3-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="d4bc3-114">Leia as propriedades e os relacionamentos do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d4bc3-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="d4bc3-115">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="d4bc3-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="d4bc3-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="d4bc3-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="d4bc3-117">Atualize as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d4bc3-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4bc3-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4bc3-118">Properties</span></span>
|<span data-ttu-id="d4bc3-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4bc3-119">Property</span></span>|<span data-ttu-id="d4bc3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4bc3-120">Type</span></span>|<span data-ttu-id="d4bc3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4bc3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4bc3-122">id</span><span class="sxs-lookup"><span data-stu-id="d4bc3-122">id</span></span>|<span data-ttu-id="d4bc3-123">String</span><span class="sxs-lookup"><span data-stu-id="d4bc3-123">String</span></span>|<span data-ttu-id="d4bc3-124">Chave da entidade Windows management app integridade resumida.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="d4bc3-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4bc3-125">healthyDeviceCount</span></span>|<span data-ttu-id="d4bc3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d4bc3-126">Int32</span></span>|<span data-ttu-id="d4bc3-127">Contagem de dispositivo íntegro.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-127">Healthy device count.</span></span>|
|<span data-ttu-id="d4bc3-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4bc3-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="d4bc3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d4bc3-129">Int32</span></span>|<span data-ttu-id="d4bc3-130">Contagem de dispositivo não íntegros.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="d4bc3-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4bc3-131">unknownDeviceCount</span></span>|<span data-ttu-id="d4bc3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d4bc3-132">Int32</span></span>|<span data-ttu-id="d4bc3-133">Contagem de dispositivo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4bc3-134">Relações</span><span class="sxs-lookup"><span data-stu-id="d4bc3-134">Relationships</span></span>
<span data-ttu-id="d4bc3-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4bc3-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d4bc3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4bc3-136">JSON Representation</span></span>
<span data-ttu-id="d4bc3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4bc3-137">Here is a JSON representation of the resource.</span></span>
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





