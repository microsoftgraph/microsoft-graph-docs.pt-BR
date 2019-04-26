---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962e759e83b08baf7fc150e07dc84ed7146feb0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563851"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="1a49a-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="1a49a-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="1a49a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a49a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a49a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a49a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a49a-106">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="1a49a-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="1a49a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1a49a-107">Members</span></span>
|<span data-ttu-id="1a49a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1a49a-108">Member</span></span>|<span data-ttu-id="1a49a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1a49a-109">Value</span></span>|<span data-ttu-id="1a49a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a49a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a49a-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="1a49a-111">useDeviceSettings</span></span>|<span data-ttu-id="1a49a-112">,0</span><span class="sxs-lookup"><span data-stu-id="1a49a-112">0</span></span>|<span data-ttu-id="1a49a-113">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a49a-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="1a49a-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="1a49a-114">afterDeviceRestart</span></span>|<span data-ttu-id="1a49a-115">1 </span><span class="sxs-lookup"><span data-stu-id="1a49a-115">1</span></span>|<span data-ttu-id="1a49a-116">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="1a49a-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="1a49a-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="1a49a-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="1a49a-118">2 </span><span class="sxs-lookup"><span data-stu-id="1a49a-118">2</span></span>|<span data-ttu-id="1a49a-119">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="1a49a-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="1a49a-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="1a49a-120">whenDeviceLocked</span></span>|<span data-ttu-id="1a49a-121">3 </span><span class="sxs-lookup"><span data-stu-id="1a49a-121">3</span></span>|<span data-ttu-id="1a49a-122">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="1a49a-122">App data associated with this policy is encrypted when the device is locked</span></span>|





