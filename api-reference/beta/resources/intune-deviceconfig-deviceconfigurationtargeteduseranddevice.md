---
title: tipo de recurso de deviceConfigurationTargetedUserAndDevice
description: Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410739"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="41647-103">tipo de recurso de deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="41647-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="41647-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="41647-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="41647-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41647-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41647-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="41647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41647-107">Resumo de um conjunto de políticas de configuração de dispositivo de conflito.</span><span class="sxs-lookup"><span data-stu-id="41647-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="41647-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41647-108">Properties</span></span>
|<span data-ttu-id="41647-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41647-109">Property</span></span>|<span data-ttu-id="41647-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41647-110">Type</span></span>|<span data-ttu-id="41647-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41647-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41647-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="41647-112">deviceId</span></span>|<span data-ttu-id="41647-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41647-113">String</span></span>|<span data-ttu-id="41647-114">A id do dispositivo em que o check-in.</span><span class="sxs-lookup"><span data-stu-id="41647-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="41647-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="41647-115">deviceName</span></span>|<span data-ttu-id="41647-116">String</span><span class="sxs-lookup"><span data-stu-id="41647-116">String</span></span>|<span data-ttu-id="41647-117">O nome do dispositivo em que o check-in.</span><span class="sxs-lookup"><span data-stu-id="41647-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="41647-118">userId</span><span class="sxs-lookup"><span data-stu-id="41647-118">userId</span></span>|<span data-ttu-id="41647-119">String</span><span class="sxs-lookup"><span data-stu-id="41647-119">String</span></span>|<span data-ttu-id="41647-120">A identificação do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="41647-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="41647-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="41647-121">userDisplayName</span></span>|<span data-ttu-id="41647-122">String</span><span class="sxs-lookup"><span data-stu-id="41647-122">String</span></span>|<span data-ttu-id="41647-123">O nome de exibição do usuário no check-in</span><span class="sxs-lookup"><span data-stu-id="41647-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="41647-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41647-124">userPrincipalName</span></span>|<span data-ttu-id="41647-125">String</span><span class="sxs-lookup"><span data-stu-id="41647-125">String</span></span>|<span data-ttu-id="41647-126">O UPN do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="41647-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="41647-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="41647-127">lastCheckinDateTime</span></span>|<span data-ttu-id="41647-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41647-128">DateTimeOffset</span></span>|<span data-ttu-id="41647-129">Última hora de check-in para este par de dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="41647-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41647-130">Relações</span><span class="sxs-lookup"><span data-stu-id="41647-130">Relationships</span></span>
<span data-ttu-id="41647-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41647-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41647-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41647-132">JSON Representation</span></span>
<span data-ttu-id="41647-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41647-133">Here is a JSON representation of the resource.</span></span>
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




