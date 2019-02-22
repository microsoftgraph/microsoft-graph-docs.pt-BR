---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159077"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="ee80c-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="ee80c-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="ee80c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee80c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee80c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee80c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee80c-106">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ee80c-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="ee80c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ee80c-107">Members</span></span>
|<span data-ttu-id="ee80c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ee80c-108">Member</span></span>|<span data-ttu-id="ee80c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ee80c-109">Value</span></span>|<span data-ttu-id="ee80c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee80c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee80c-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="ee80c-111">useDeviceSettings</span></span>|<span data-ttu-id="ee80c-112">,0</span><span class="sxs-lookup"><span data-stu-id="ee80c-112">0</span></span>|<span data-ttu-id="ee80c-113">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee80c-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="ee80c-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="ee80c-114">afterDeviceRestart</span></span>|<span data-ttu-id="ee80c-115">1</span><span class="sxs-lookup"><span data-stu-id="ee80c-115">1</span></span>|<span data-ttu-id="ee80c-116">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="ee80c-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="ee80c-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="ee80c-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="ee80c-118">duas</span><span class="sxs-lookup"><span data-stu-id="ee80c-118">2</span></span>|<span data-ttu-id="ee80c-119">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="ee80c-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="ee80c-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="ee80c-120">whenDeviceLocked</span></span>|<span data-ttu-id="ee80c-121">3D</span><span class="sxs-lookup"><span data-stu-id="ee80c-121">3</span></span>|<span data-ttu-id="ee80c-122">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="ee80c-122">App data associated with this policy is encrypted when the device is locked</span></span>|




