---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
ms.openlocfilehash: 6bd23f6cd590724c2c981ddf2c3087ead4c21817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326114"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="3938c-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="3938c-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="3938c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3938c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3938c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3938c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3938c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3938c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3938c-107">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3938c-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="3938c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3938c-108">Members</span></span>
|<span data-ttu-id="3938c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3938c-109">Member</span></span>|<span data-ttu-id="3938c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3938c-110">Value</span></span>|<span data-ttu-id="3938c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3938c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3938c-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="3938c-112">useDeviceSettings</span></span>|<span data-ttu-id="3938c-113">0</span><span class="sxs-lookup"><span data-stu-id="3938c-113">0</span></span>|<span data-ttu-id="3938c-114">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3938c-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="3938c-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="3938c-115">afterDeviceRestart</span></span>|<span data-ttu-id="3938c-116">1</span><span class="sxs-lookup"><span data-stu-id="3938c-116">1</span></span>|<span data-ttu-id="3938c-117">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="3938c-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="3938c-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="3938c-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="3938c-119">2</span><span class="sxs-lookup"><span data-stu-id="3938c-119">2</span></span>|<span data-ttu-id="3938c-120">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="3938c-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="3938c-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="3938c-121">whenDeviceLocked</span></span>|<span data-ttu-id="3938c-122">3</span><span class="sxs-lookup"><span data-stu-id="3938c-122">3</span></span>|<span data-ttu-id="3938c-123">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="3938c-123">App data associated with this policy is encrypted when the device is locked</span></span>|





