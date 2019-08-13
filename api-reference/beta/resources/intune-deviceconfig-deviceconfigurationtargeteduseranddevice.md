---
title: tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d994491b86d1590c5765d5771ea52b24d6e42f8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332929"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="89a17-103">tipo de recurso deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="89a17-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="89a17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89a17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89a17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89a17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89a17-106">Resumo de conflito para um conjunto de políticas de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89a17-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="89a17-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89a17-107">Properties</span></span>
|<span data-ttu-id="89a17-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89a17-108">Property</span></span>|<span data-ttu-id="89a17-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="89a17-109">Type</span></span>|<span data-ttu-id="89a17-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a17-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="89a17-111">deviceId</span></span>|<span data-ttu-id="89a17-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89a17-112">String</span></span>|<span data-ttu-id="89a17-113">A ID do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="89a17-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="89a17-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="89a17-114">deviceName</span></span>|<span data-ttu-id="89a17-115">String</span><span class="sxs-lookup"><span data-stu-id="89a17-115">String</span></span>|<span data-ttu-id="89a17-116">O nome do dispositivo no check-in.</span><span class="sxs-lookup"><span data-stu-id="89a17-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="89a17-117">userId</span><span class="sxs-lookup"><span data-stu-id="89a17-117">userId</span></span>|<span data-ttu-id="89a17-118">String</span><span class="sxs-lookup"><span data-stu-id="89a17-118">String</span></span>|<span data-ttu-id="89a17-119">A ID do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="89a17-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="89a17-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="89a17-120">userDisplayName</span></span>|<span data-ttu-id="89a17-121">String</span><span class="sxs-lookup"><span data-stu-id="89a17-121">String</span></span>|<span data-ttu-id="89a17-122">O nome de exibição do usuário no check-in</span><span class="sxs-lookup"><span data-stu-id="89a17-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="89a17-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89a17-123">userPrincipalName</span></span>|<span data-ttu-id="89a17-124">String</span><span class="sxs-lookup"><span data-stu-id="89a17-124">String</span></span>|<span data-ttu-id="89a17-125">O UPN do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="89a17-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="89a17-126">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="89a17-126">lastCheckinDateTime</span></span>|<span data-ttu-id="89a17-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89a17-127">DateTimeOffset</span></span>|<span data-ttu-id="89a17-128">Horário da última verificação para este par de usuários/dispositivos.</span><span class="sxs-lookup"><span data-stu-id="89a17-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89a17-129">Relações</span><span class="sxs-lookup"><span data-stu-id="89a17-129">Relationships</span></span>
<span data-ttu-id="89a17-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89a17-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89a17-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89a17-131">JSON Representation</span></span>
<span data-ttu-id="89a17-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89a17-132">Here is a JSON representation of the resource.</span></span>
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



