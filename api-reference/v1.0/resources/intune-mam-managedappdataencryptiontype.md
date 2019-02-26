---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256767"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="19687-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="19687-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="19687-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19687-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19687-105">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="19687-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="19687-106">Membros</span><span class="sxs-lookup"><span data-stu-id="19687-106">Members</span></span>
|<span data-ttu-id="19687-107">Membro</span><span class="sxs-lookup"><span data-stu-id="19687-107">Member</span></span>|<span data-ttu-id="19687-108">Valor</span><span class="sxs-lookup"><span data-stu-id="19687-108">Value</span></span>|<span data-ttu-id="19687-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="19687-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19687-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="19687-110">useDeviceSettings</span></span>|<span data-ttu-id="19687-111">,0</span><span class="sxs-lookup"><span data-stu-id="19687-111">0</span></span>|<span data-ttu-id="19687-112">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19687-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="19687-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="19687-113">afterDeviceRestart</span></span>|<span data-ttu-id="19687-114">1</span><span class="sxs-lookup"><span data-stu-id="19687-114">1</span></span>|<span data-ttu-id="19687-115">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="19687-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="19687-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="19687-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="19687-117">duas</span><span class="sxs-lookup"><span data-stu-id="19687-117">2</span></span>|<span data-ttu-id="19687-118">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="19687-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="19687-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="19687-119">whenDeviceLocked</span></span>|<span data-ttu-id="19687-120">3D</span><span class="sxs-lookup"><span data-stu-id="19687-120">3</span></span>|<span data-ttu-id="19687-121">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="19687-121">App data associated with this policy is encrypted when the device is locked</span></span>|



