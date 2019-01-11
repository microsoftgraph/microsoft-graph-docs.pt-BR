---
title: tipo de recurso de windowsManagementAppHealthSummary
description: Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40ba93025059a85a11b061464d04bca4118b88bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843817"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="0b20d-103">tipo de recurso de windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="0b20d-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="0b20d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b20d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b20d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b20d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b20d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b20d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b20d-107">Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="0b20d-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="0b20d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b20d-108">Methods</span></span>
|<span data-ttu-id="0b20d-109">Método</span><span class="sxs-lookup"><span data-stu-id="0b20d-109">Method</span></span>|<span data-ttu-id="0b20d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b20d-110">Return Type</span></span>|<span data-ttu-id="0b20d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b20d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b20d-112">Obter windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="0b20d-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="0b20d-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="0b20d-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="0b20d-114">Leia as propriedades e os relacionamentos do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0b20d-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="0b20d-115">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="0b20d-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="0b20d-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="0b20d-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="0b20d-117">Atualize as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0b20d-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b20d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b20d-118">Properties</span></span>
|<span data-ttu-id="0b20d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b20d-119">Property</span></span>|<span data-ttu-id="0b20d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b20d-120">Type</span></span>|<span data-ttu-id="0b20d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b20d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b20d-122">id</span><span class="sxs-lookup"><span data-stu-id="0b20d-122">id</span></span>|<span data-ttu-id="0b20d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b20d-123">String</span></span>|<span data-ttu-id="0b20d-124">Chave da entidade Windows management app integridade resumida.</span><span class="sxs-lookup"><span data-stu-id="0b20d-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="0b20d-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b20d-125">healthyDeviceCount</span></span>|<span data-ttu-id="0b20d-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0b20d-126">Int32</span></span>|<span data-ttu-id="0b20d-127">Contagem de dispositivo íntegro.</span><span class="sxs-lookup"><span data-stu-id="0b20d-127">Healthy device count.</span></span>|
|<span data-ttu-id="0b20d-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b20d-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="0b20d-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0b20d-129">Int32</span></span>|<span data-ttu-id="0b20d-130">Contagem de dispositivo não íntegros.</span><span class="sxs-lookup"><span data-stu-id="0b20d-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="0b20d-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b20d-131">unknownDeviceCount</span></span>|<span data-ttu-id="0b20d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0b20d-132">Int32</span></span>|<span data-ttu-id="0b20d-133">Contagem de dispositivo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="0b20d-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b20d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="0b20d-134">Relationships</span></span>
<span data-ttu-id="0b20d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b20d-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b20d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b20d-136">JSON Representation</span></span>
<span data-ttu-id="0b20d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b20d-137">Here is a JSON representation of the resource.</span></span>
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





