---
title: tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c722cf1a21e46ec6066efc1e836793d77ce8e8b7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199389"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="99983-103">tipo de recurso deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="99983-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="99983-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99983-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99983-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99983-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99983-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99983-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99983-107">Resumo de conflito para um conjunto de políticas de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99983-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="99983-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99983-108">Properties</span></span>
|<span data-ttu-id="99983-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99983-109">Property</span></span>|<span data-ttu-id="99983-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="99983-110">Type</span></span>|<span data-ttu-id="99983-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99983-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99983-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="99983-112">deviceId</span></span>|<span data-ttu-id="99983-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99983-113">String</span></span>|<span data-ttu-id="99983-114">A ID do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="99983-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="99983-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="99983-115">deviceName</span></span>|<span data-ttu-id="99983-116">String</span><span class="sxs-lookup"><span data-stu-id="99983-116">String</span></span>|<span data-ttu-id="99983-117">O nome do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="99983-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="99983-118">userId</span><span class="sxs-lookup"><span data-stu-id="99983-118">userId</span></span>|<span data-ttu-id="99983-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99983-119">String</span></span>|<span data-ttu-id="99983-120">A ID do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="99983-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="99983-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="99983-121">userDisplayName</span></span>|<span data-ttu-id="99983-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99983-122">String</span></span>|<span data-ttu-id="99983-123">O nome de exibição do usuário no check-in</span><span class="sxs-lookup"><span data-stu-id="99983-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="99983-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99983-124">userPrincipalName</span></span>|<span data-ttu-id="99983-125">String</span><span class="sxs-lookup"><span data-stu-id="99983-125">String</span></span>|<span data-ttu-id="99983-126">O UPN do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="99983-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="99983-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="99983-127">lastCheckinDateTime</span></span>|<span data-ttu-id="99983-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99983-128">DateTimeOffset</span></span>|<span data-ttu-id="99983-129">Horário da última verificação para este par de usuários/dispositivos.</span><span class="sxs-lookup"><span data-stu-id="99983-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99983-130">Relações</span><span class="sxs-lookup"><span data-stu-id="99983-130">Relationships</span></span>
<span data-ttu-id="99983-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99983-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99983-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99983-132">JSON Representation</span></span>
<span data-ttu-id="99983-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99983-133">Here is a JSON representation of the resource.</span></span>
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




