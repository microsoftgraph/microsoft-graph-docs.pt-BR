---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e02d2dd993a31056a19d4c54155b1195e93ab58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074955"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="07d31-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="07d31-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="07d31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07d31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07d31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d31-106">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="07d31-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="07d31-107">Membros</span><span class="sxs-lookup"><span data-stu-id="07d31-107">Members</span></span>
|<span data-ttu-id="07d31-108">Membro</span><span class="sxs-lookup"><span data-stu-id="07d31-108">Member</span></span>|<span data-ttu-id="07d31-109">Valor</span><span class="sxs-lookup"><span data-stu-id="07d31-109">Value</span></span>|<span data-ttu-id="07d31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07d31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d31-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="07d31-111">useDeviceSettings</span></span>|<span data-ttu-id="07d31-112">,0</span><span class="sxs-lookup"><span data-stu-id="07d31-112">0</span></span>|<span data-ttu-id="07d31-113">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d31-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="07d31-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="07d31-114">afterDeviceRestart</span></span>|<span data-ttu-id="07d31-115">1 </span><span class="sxs-lookup"><span data-stu-id="07d31-115">1</span></span>|<span data-ttu-id="07d31-116">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="07d31-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="07d31-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="07d31-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="07d31-118">2 </span><span class="sxs-lookup"><span data-stu-id="07d31-118">2</span></span>|<span data-ttu-id="07d31-119">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="07d31-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="07d31-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="07d31-120">whenDeviceLocked</span></span>|<span data-ttu-id="07d31-121">3D</span><span class="sxs-lookup"><span data-stu-id="07d31-121">3</span></span>|<span data-ttu-id="07d31-122">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="07d31-122">App data associated with this policy is encrypted when the device is locked</span></span>|









