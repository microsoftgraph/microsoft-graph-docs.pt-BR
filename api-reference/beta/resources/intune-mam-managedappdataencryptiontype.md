---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1bc52b0fa05a65adfb3e195d0a38c9bebd78e6c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267030"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="42999-103">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="42999-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="42999-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42999-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42999-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42999-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42999-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42999-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42999-107">Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="42999-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="42999-108">Membros</span><span class="sxs-lookup"><span data-stu-id="42999-108">Members</span></span>
|<span data-ttu-id="42999-109">Membro</span><span class="sxs-lookup"><span data-stu-id="42999-109">Member</span></span>|<span data-ttu-id="42999-110">Valor</span><span class="sxs-lookup"><span data-stu-id="42999-110">Value</span></span>|<span data-ttu-id="42999-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42999-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42999-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="42999-112">useDeviceSettings</span></span>|<span data-ttu-id="42999-113">,0</span><span class="sxs-lookup"><span data-stu-id="42999-113">0</span></span>|<span data-ttu-id="42999-114">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42999-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="42999-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="42999-115">afterDeviceRestart</span></span>|<span data-ttu-id="42999-116">1</span><span class="sxs-lookup"><span data-stu-id="42999-116">1</span></span>|<span data-ttu-id="42999-117">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="42999-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="42999-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="42999-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="42999-119">duas</span><span class="sxs-lookup"><span data-stu-id="42999-119">2</span></span>|<span data-ttu-id="42999-120">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="42999-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="42999-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="42999-121">whenDeviceLocked</span></span>|<span data-ttu-id="42999-122">3D</span><span class="sxs-lookup"><span data-stu-id="42999-122">3</span></span>|<span data-ttu-id="42999-123">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="42999-123">App data associated with this policy is encrypted when the device is locked</span></span>|




