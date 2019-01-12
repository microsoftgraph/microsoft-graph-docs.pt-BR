---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4417d488a1590f8d8e9c40e13118e6ef0dc044d1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944429"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="e7317-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="e7317-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="e7317-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7317-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7317-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7317-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e7317-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7317-107">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e7317-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="e7317-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e7317-108">Members</span></span>
|<span data-ttu-id="e7317-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e7317-109">Member</span></span>|<span data-ttu-id="e7317-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e7317-110">Value</span></span>|<span data-ttu-id="e7317-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7317-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7317-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="e7317-112">useDeviceSettings</span></span>|<span data-ttu-id="e7317-113">0</span><span class="sxs-lookup"><span data-stu-id="e7317-113">0</span></span>|<span data-ttu-id="e7317-114">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e7317-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="e7317-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="e7317-115">afterDeviceRestart</span></span>|<span data-ttu-id="e7317-116">1</span><span class="sxs-lookup"><span data-stu-id="e7317-116">1</span></span>|<span data-ttu-id="e7317-117">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="e7317-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="e7317-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="e7317-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="e7317-119">2</span><span class="sxs-lookup"><span data-stu-id="e7317-119">2</span></span>|<span data-ttu-id="e7317-120">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="e7317-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="e7317-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e7317-121">whenDeviceLocked</span></span>|<span data-ttu-id="e7317-122">3</span><span class="sxs-lookup"><span data-stu-id="e7317-122">3</span></span>|<span data-ttu-id="e7317-123">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="e7317-123">App data associated with this policy is encrypted when the device is locked</span></span>|





