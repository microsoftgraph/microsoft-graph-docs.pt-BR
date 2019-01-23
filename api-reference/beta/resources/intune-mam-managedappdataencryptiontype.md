---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413686"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="8b35f-103">tipo de enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="8b35f-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="8b35f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b35f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b35f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b35f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b35f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8b35f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b35f-107">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="8b35f-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="8b35f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8b35f-108">Members</span></span>
|<span data-ttu-id="8b35f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8b35f-109">Member</span></span>|<span data-ttu-id="8b35f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8b35f-110">Value</span></span>|<span data-ttu-id="8b35f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b35f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b35f-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="8b35f-112">useDeviceSettings</span></span>|<span data-ttu-id="8b35f-113">0</span><span class="sxs-lookup"><span data-stu-id="8b35f-113">0</span></span>|<span data-ttu-id="8b35f-114">Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b35f-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="8b35f-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="8b35f-115">afterDeviceRestart</span></span>|<span data-ttu-id="8b35f-116">1</span><span class="sxs-lookup"><span data-stu-id="8b35f-116">1</span></span>|<span data-ttu-id="8b35f-117">Dados de aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="8b35f-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="8b35f-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="8b35f-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="8b35f-119">2</span><span class="sxs-lookup"><span data-stu-id="8b35f-119">2</span></span>|<span data-ttu-id="8b35f-120">Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="8b35f-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="8b35f-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="8b35f-121">whenDeviceLocked</span></span>|<span data-ttu-id="8b35f-122">3</span><span class="sxs-lookup"><span data-stu-id="8b35f-122">3</span></span>|<span data-ttu-id="8b35f-123">Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado</span><span class="sxs-lookup"><span data-stu-id="8b35f-123">App data associated with this policy is encrypted when the device is locked</span></span>|




