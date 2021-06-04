---
title: Tipo denum managedAppDataEncryptionType
description: Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a3cbe74f8dbc81330b899b4acedcbc880b8d81d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754494"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="b4c3a-103">Tipo denum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="b4c3a-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="b4c3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4c3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4c3a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4c3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c3a-106">Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b4c3a-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="b4c3a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b4c3a-107">Members</span></span>
|<span data-ttu-id="b4c3a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b4c3a-108">Member</span></span>|<span data-ttu-id="b4c3a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b4c3a-109">Value</span></span>|<span data-ttu-id="b4c3a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4c3a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c3a-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="b4c3a-111">useDeviceSettings</span></span>|<span data-ttu-id="b4c3a-112">0</span><span class="sxs-lookup"><span data-stu-id="b4c3a-112">0</span></span>|<span data-ttu-id="b4c3a-113">Os dados do aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4c3a-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="b4c3a-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="b4c3a-114">afterDeviceRestart</span></span>|<span data-ttu-id="b4c3a-115">1</span><span class="sxs-lookup"><span data-stu-id="b4c3a-115">1</span></span>|<span data-ttu-id="b4c3a-116">Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="b4c3a-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="b4c3a-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="b4c3a-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="b4c3a-118">2</span><span class="sxs-lookup"><span data-stu-id="b4c3a-118">2</span></span>|<span data-ttu-id="b4c3a-119">Os dados do aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado, exceto dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="b4c3a-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="b4c3a-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="b4c3a-120">whenDeviceLocked</span></span>|<span data-ttu-id="b4c3a-121">3</span><span class="sxs-lookup"><span data-stu-id="b4c3a-121">3</span></span>|<span data-ttu-id="b4c3a-122">Os dados do aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado</span><span class="sxs-lookup"><span data-stu-id="b4c3a-122">App data associated with this policy is encrypted when the device is locked</span></span>|




