---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b92f2f9d4d1cfa095bae4a51fc459fee8980d60
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373363"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="136e5-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="136e5-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="136e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="136e5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="136e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="136e5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="136e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="136e5-107">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="136e5-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="136e5-108">Membros</span><span class="sxs-lookup"><span data-stu-id="136e5-108">Members</span></span>
|<span data-ttu-id="136e5-109">Membro</span><span class="sxs-lookup"><span data-stu-id="136e5-109">Member</span></span>|<span data-ttu-id="136e5-110">Valor</span><span class="sxs-lookup"><span data-stu-id="136e5-110">Value</span></span>|<span data-ttu-id="136e5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="136e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="136e5-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="136e5-112">useDeviceSettings</span></span>|<span data-ttu-id="136e5-113">,0</span><span class="sxs-lookup"><span data-stu-id="136e5-113">0</span></span>|<span data-ttu-id="136e5-114">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="136e5-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="136e5-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="136e5-115">afterDeviceRestart</span></span>|<span data-ttu-id="136e5-116">1</span><span class="sxs-lookup"><span data-stu-id="136e5-116">1</span></span>|<span data-ttu-id="136e5-117">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="136e5-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="136e5-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="136e5-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="136e5-119">duas</span><span class="sxs-lookup"><span data-stu-id="136e5-119">2</span></span>|<span data-ttu-id="136e5-120">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="136e5-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="136e5-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="136e5-121">whenDeviceLocked</span></span>|<span data-ttu-id="136e5-122">3D</span><span class="sxs-lookup"><span data-stu-id="136e5-122">3</span></span>|<span data-ttu-id="136e5-123">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="136e5-123">App data associated with this policy is encrypted when the device is locked</span></span>|



