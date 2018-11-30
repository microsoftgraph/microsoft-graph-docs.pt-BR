---
title: tipo de recurso de deviceConfigurationTargetedUserAndDevice
description: Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
ms.openlocfilehash: 6f79a8fe24e06d2bdafa81c30cabf8158b4e5773
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033978"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="8c704-103">tipo de recurso de deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="8c704-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="8c704-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c704-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c704-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c704-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c704-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c704-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c704-107">Resumo de um conjunto de políticas de configuração de dispositivo de conflito.</span><span class="sxs-lookup"><span data-stu-id="8c704-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="8c704-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c704-108">Properties</span></span>
|<span data-ttu-id="8c704-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c704-109">Property</span></span>|<span data-ttu-id="8c704-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c704-110">Type</span></span>|<span data-ttu-id="8c704-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c704-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c704-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="8c704-112">deviceId</span></span>|<span data-ttu-id="8c704-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c704-113">String</span></span>|<span data-ttu-id="8c704-114">A id do dispositivo em que o check-in.</span><span class="sxs-lookup"><span data-stu-id="8c704-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="8c704-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="8c704-115">deviceName</span></span>|<span data-ttu-id="8c704-116">String</span><span class="sxs-lookup"><span data-stu-id="8c704-116">String</span></span>|<span data-ttu-id="8c704-117">O nome do dispositivo em que o check-in.</span><span class="sxs-lookup"><span data-stu-id="8c704-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="8c704-118">userId</span><span class="sxs-lookup"><span data-stu-id="8c704-118">userId</span></span>|<span data-ttu-id="8c704-119">String</span><span class="sxs-lookup"><span data-stu-id="8c704-119">String</span></span>|<span data-ttu-id="8c704-120">A identificação do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="8c704-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="8c704-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8c704-121">userDisplayName</span></span>|<span data-ttu-id="8c704-122">String</span><span class="sxs-lookup"><span data-stu-id="8c704-122">String</span></span>|<span data-ttu-id="8c704-123">O nome de exibição do usuário no check-in</span><span class="sxs-lookup"><span data-stu-id="8c704-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="8c704-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c704-124">userPrincipalName</span></span>|<span data-ttu-id="8c704-125">String</span><span class="sxs-lookup"><span data-stu-id="8c704-125">String</span></span>|<span data-ttu-id="8c704-126">O UPN do usuário no check-in.</span><span class="sxs-lookup"><span data-stu-id="8c704-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="8c704-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="8c704-127">lastCheckinDateTime</span></span>|<span data-ttu-id="8c704-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c704-128">DateTimeOffset</span></span>|<span data-ttu-id="8c704-129">Última hora de check-in para este par de dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8c704-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c704-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8c704-130">Relationships</span></span>
<span data-ttu-id="8c704-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c704-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c704-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c704-132">JSON Representation</span></span>
<span data-ttu-id="8c704-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c704-133">Here is a JSON representation of the resource.</span></span>
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





