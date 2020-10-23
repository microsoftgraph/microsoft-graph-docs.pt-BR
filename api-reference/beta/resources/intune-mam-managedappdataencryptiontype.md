---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e57afb0a878248e761d11434825f1d0c9403a6c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684621"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="438f3-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="438f3-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="438f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="438f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="438f3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="438f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="438f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="438f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438f3-107">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="438f3-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="438f3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="438f3-108">Members</span></span>
|<span data-ttu-id="438f3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="438f3-109">Member</span></span>|<span data-ttu-id="438f3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="438f3-110">Value</span></span>|<span data-ttu-id="438f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="438f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438f3-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="438f3-112">useDeviceSettings</span></span>|<span data-ttu-id="438f3-113">,0</span><span class="sxs-lookup"><span data-stu-id="438f3-113">0</span></span>|<span data-ttu-id="438f3-114">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="438f3-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="438f3-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="438f3-115">afterDeviceRestart</span></span>|<span data-ttu-id="438f3-116">1</span><span class="sxs-lookup"><span data-stu-id="438f3-116">1</span></span>|<span data-ttu-id="438f3-117">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="438f3-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="438f3-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="438f3-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="438f3-119">duas</span><span class="sxs-lookup"><span data-stu-id="438f3-119">2</span></span>|<span data-ttu-id="438f3-120">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="438f3-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="438f3-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="438f3-121">whenDeviceLocked</span></span>|<span data-ttu-id="438f3-122">3D</span><span class="sxs-lookup"><span data-stu-id="438f3-122">3</span></span>|<span data-ttu-id="438f3-123">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="438f3-123">App data associated with this policy is encrypted when the device is locked</span></span>|





