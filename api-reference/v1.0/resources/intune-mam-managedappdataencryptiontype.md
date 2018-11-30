---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006267"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="dc9a1-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="dc9a1-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="dc9a1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dc9a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc9a1-105">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="dc9a1-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="dc9a1-106">Membros</span><span class="sxs-lookup"><span data-stu-id="dc9a1-106">Members</span></span>
|<span data-ttu-id="dc9a1-107">Membro</span><span class="sxs-lookup"><span data-stu-id="dc9a1-107">Member</span></span>|<span data-ttu-id="dc9a1-108">Valor</span><span class="sxs-lookup"><span data-stu-id="dc9a1-108">Value</span></span>|<span data-ttu-id="dc9a1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc9a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc9a1-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="dc9a1-110">useDeviceSettings</span></span>|<span data-ttu-id="dc9a1-111">0</span><span class="sxs-lookup"><span data-stu-id="dc9a1-111">0</span></span>|<span data-ttu-id="dc9a1-112">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc9a1-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="dc9a1-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="dc9a1-113">afterDeviceRestart</span></span>|<span data-ttu-id="dc9a1-114">1</span><span class="sxs-lookup"><span data-stu-id="dc9a1-114">1</span></span>|<span data-ttu-id="dc9a1-115">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="dc9a1-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="dc9a1-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="dc9a1-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="dc9a1-117">2</span><span class="sxs-lookup"><span data-stu-id="dc9a1-117">2</span></span>|<span data-ttu-id="dc9a1-118">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="dc9a1-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="dc9a1-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="dc9a1-119">whenDeviceLocked</span></span>|<span data-ttu-id="dc9a1-120">3</span><span class="sxs-lookup"><span data-stu-id="dc9a1-120">3</span></span>|<span data-ttu-id="dc9a1-121">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="dc9a1-121">App data associated with this policy is encrypted when the device is locked</span></span>|



