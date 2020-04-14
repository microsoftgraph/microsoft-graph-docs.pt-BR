---
title: tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a553cf15a82b25d78eb983037d45c1c3c245025
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469364"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="bb804-103">tipo de recurso deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="bb804-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="bb804-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb804-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb804-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb804-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb804-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb804-107">Resumo de conflito para um conjunto de políticas de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb804-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="bb804-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb804-108">Properties</span></span>
|<span data-ttu-id="bb804-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb804-109">Property</span></span>|<span data-ttu-id="bb804-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb804-110">Type</span></span>|<span data-ttu-id="bb804-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb804-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb804-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="bb804-112">deviceId</span></span>|<span data-ttu-id="bb804-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb804-113">String</span></span>|<span data-ttu-id="bb804-114">A ID do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="bb804-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="bb804-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="bb804-115">deviceName</span></span>|<span data-ttu-id="bb804-116">String</span><span class="sxs-lookup"><span data-stu-id="bb804-116">String</span></span>|<span data-ttu-id="bb804-117">O nome do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="bb804-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="bb804-118">userId</span><span class="sxs-lookup"><span data-stu-id="bb804-118">userId</span></span>|<span data-ttu-id="bb804-119">String</span><span class="sxs-lookup"><span data-stu-id="bb804-119">String</span></span>|<span data-ttu-id="bb804-120">A ID do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="bb804-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="bb804-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb804-121">userDisplayName</span></span>|<span data-ttu-id="bb804-122">String</span><span class="sxs-lookup"><span data-stu-id="bb804-122">String</span></span>|<span data-ttu-id="bb804-123">O nome de exibição do usuário no check-in</span><span class="sxs-lookup"><span data-stu-id="bb804-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="bb804-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb804-124">userPrincipalName</span></span>|<span data-ttu-id="bb804-125">String</span><span class="sxs-lookup"><span data-stu-id="bb804-125">String</span></span>|<span data-ttu-id="bb804-126">O UPN do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="bb804-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="bb804-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="bb804-127">lastCheckinDateTime</span></span>|<span data-ttu-id="bb804-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb804-128">DateTimeOffset</span></span>|<span data-ttu-id="bb804-129">Horário da última verificação para este par de usuários/dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bb804-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb804-130">Relações</span><span class="sxs-lookup"><span data-stu-id="bb804-130">Relationships</span></span>
<span data-ttu-id="bb804-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb804-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb804-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb804-132">JSON Representation</span></span>
<span data-ttu-id="bb804-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb804-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```



