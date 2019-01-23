---
title: tipo de recurso de windowsManagementAppHealthSummary
description: Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ca46f61259b8b956439c541bf8d5703a35aa93b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393848"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="990d8-103">tipo de recurso de windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="990d8-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="990d8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="990d8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="990d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="990d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="990d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="990d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="990d8-107">Contém propriedades para o resumo da integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="990d8-107">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="990d8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="990d8-108">Methods</span></span>
|<span data-ttu-id="990d8-109">Método</span><span class="sxs-lookup"><span data-stu-id="990d8-109">Method</span></span>|<span data-ttu-id="990d8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="990d8-110">Return Type</span></span>|<span data-ttu-id="990d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="990d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="990d8-112">Obter windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="990d8-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="990d8-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="990d8-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="990d8-114">Leia as propriedades e os relacionamentos do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="990d8-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="990d8-115">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="990d8-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="990d8-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="990d8-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="990d8-117">Atualize as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="990d8-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="990d8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="990d8-118">Properties</span></span>
|<span data-ttu-id="990d8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="990d8-119">Property</span></span>|<span data-ttu-id="990d8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="990d8-120">Type</span></span>|<span data-ttu-id="990d8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="990d8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="990d8-122">id</span><span class="sxs-lookup"><span data-stu-id="990d8-122">id</span></span>|<span data-ttu-id="990d8-123">String</span><span class="sxs-lookup"><span data-stu-id="990d8-123">String</span></span>|<span data-ttu-id="990d8-124">Chave da entidade Windows management app integridade resumida.</span><span class="sxs-lookup"><span data-stu-id="990d8-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="990d8-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="990d8-125">healthyDeviceCount</span></span>|<span data-ttu-id="990d8-126">Int32</span><span class="sxs-lookup"><span data-stu-id="990d8-126">Int32</span></span>|<span data-ttu-id="990d8-127">Contagem de dispositivo íntegro.</span><span class="sxs-lookup"><span data-stu-id="990d8-127">Healthy device count.</span></span>|
|<span data-ttu-id="990d8-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="990d8-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="990d8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="990d8-129">Int32</span></span>|<span data-ttu-id="990d8-130">Contagem de dispositivo não íntegros.</span><span class="sxs-lookup"><span data-stu-id="990d8-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="990d8-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="990d8-131">unknownDeviceCount</span></span>|<span data-ttu-id="990d8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="990d8-132">Int32</span></span>|<span data-ttu-id="990d8-133">Contagem de dispositivo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="990d8-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="990d8-134">Relações</span><span class="sxs-lookup"><span data-stu-id="990d8-134">Relationships</span></span>
<span data-ttu-id="990d8-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="990d8-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="990d8-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="990d8-136">JSON Representation</span></span>
<span data-ttu-id="990d8-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="990d8-137">Here is a JSON representation of the resource.</span></span>
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




