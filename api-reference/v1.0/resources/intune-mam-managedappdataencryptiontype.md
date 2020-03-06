---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c2a4c9b713d2b91645cf210df60ec8d3ba642a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533341"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="b77a5-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="b77a5-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="b77a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b77a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b77a5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b77a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77a5-106">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b77a5-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="b77a5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b77a5-107">Members</span></span>
|<span data-ttu-id="b77a5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b77a5-108">Member</span></span>|<span data-ttu-id="b77a5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b77a5-109">Value</span></span>|<span data-ttu-id="b77a5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b77a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77a5-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="b77a5-111">useDeviceSettings</span></span>|<span data-ttu-id="b77a5-112">,0</span><span class="sxs-lookup"><span data-stu-id="b77a5-112">0</span></span>|<span data-ttu-id="b77a5-113">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b77a5-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="b77a5-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="b77a5-114">afterDeviceRestart</span></span>|<span data-ttu-id="b77a5-115">1 </span><span class="sxs-lookup"><span data-stu-id="b77a5-115">1</span></span>|<span data-ttu-id="b77a5-116">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="b77a5-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="b77a5-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="b77a5-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="b77a5-118">2 </span><span class="sxs-lookup"><span data-stu-id="b77a5-118">2</span></span>|<span data-ttu-id="b77a5-119">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="b77a5-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="b77a5-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="b77a5-120">whenDeviceLocked</span></span>|<span data-ttu-id="b77a5-121">3 </span><span class="sxs-lookup"><span data-stu-id="b77a5-121">3</span></span>|<span data-ttu-id="b77a5-122">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="b77a5-122">App data associated with this policy is encrypted when the device is locked</span></span>|




