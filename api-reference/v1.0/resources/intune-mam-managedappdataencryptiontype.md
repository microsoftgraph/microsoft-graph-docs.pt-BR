---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08ac7a36e142a1d19dbaaeb0263ef095072a9e01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956812"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="c4446-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c4446-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="c4446-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c4446-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4446-105">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="c4446-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="c4446-106">Membros</span><span class="sxs-lookup"><span data-stu-id="c4446-106">Members</span></span>
|<span data-ttu-id="c4446-107">Membro</span><span class="sxs-lookup"><span data-stu-id="c4446-107">Member</span></span>|<span data-ttu-id="c4446-108">Valor</span><span class="sxs-lookup"><span data-stu-id="c4446-108">Value</span></span>|<span data-ttu-id="c4446-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4446-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4446-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="c4446-110">useDeviceSettings</span></span>|<span data-ttu-id="c4446-111">0</span><span class="sxs-lookup"><span data-stu-id="c4446-111">0</span></span>|<span data-ttu-id="c4446-112">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4446-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="c4446-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="c4446-113">afterDeviceRestart</span></span>|<span data-ttu-id="c4446-114">1</span><span class="sxs-lookup"><span data-stu-id="c4446-114">1</span></span>|<span data-ttu-id="c4446-115">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="c4446-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="c4446-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="c4446-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="c4446-117">2</span><span class="sxs-lookup"><span data-stu-id="c4446-117">2</span></span>|<span data-ttu-id="c4446-118">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="c4446-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="c4446-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="c4446-119">whenDeviceLocked</span></span>|<span data-ttu-id="c4446-120">3</span><span class="sxs-lookup"><span data-stu-id="c4446-120">3</span></span>|<span data-ttu-id="c4446-121">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="c4446-121">App data associated with this policy is encrypted when the device is locked</span></span>|



