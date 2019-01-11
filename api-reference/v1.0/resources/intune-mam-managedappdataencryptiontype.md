---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f57904d45b24f6aaae9d67394facb07692add67e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834143"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="97686-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="97686-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="97686-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97686-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97686-105">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="97686-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="97686-106">Membros</span><span class="sxs-lookup"><span data-stu-id="97686-106">Members</span></span>
|<span data-ttu-id="97686-107">Membro</span><span class="sxs-lookup"><span data-stu-id="97686-107">Member</span></span>|<span data-ttu-id="97686-108">Valor</span><span class="sxs-lookup"><span data-stu-id="97686-108">Value</span></span>|<span data-ttu-id="97686-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="97686-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97686-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="97686-110">useDeviceSettings</span></span>|<span data-ttu-id="97686-111">0</span><span class="sxs-lookup"><span data-stu-id="97686-111">0</span></span>|<span data-ttu-id="97686-112">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97686-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="97686-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="97686-113">afterDeviceRestart</span></span>|<span data-ttu-id="97686-114">1</span><span class="sxs-lookup"><span data-stu-id="97686-114">1</span></span>|<span data-ttu-id="97686-115">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="97686-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="97686-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="97686-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="97686-117">2</span><span class="sxs-lookup"><span data-stu-id="97686-117">2</span></span>|<span data-ttu-id="97686-118">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="97686-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="97686-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="97686-119">whenDeviceLocked</span></span>|<span data-ttu-id="97686-120">3</span><span class="sxs-lookup"><span data-stu-id="97686-120">3</span></span>|<span data-ttu-id="97686-121">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="97686-121">App data associated with this policy is encrypted when the device is locked</span></span>|



