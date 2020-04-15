---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aa66c84b04c51af52ad8f0054639c5f98cb9c665
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449122"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="d33aa-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="d33aa-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="d33aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d33aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d33aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d33aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d33aa-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="d33aa-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="d33aa-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d33aa-107">Members</span></span>
|<span data-ttu-id="d33aa-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d33aa-108">Member</span></span>|<span data-ttu-id="d33aa-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d33aa-109">Value</span></span>|<span data-ttu-id="d33aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d33aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d33aa-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="d33aa-111">userDefined</span></span>|<span data-ttu-id="d33aa-112">,0</span><span class="sxs-lookup"><span data-stu-id="d33aa-112">0</span></span>|<span data-ttu-id="d33aa-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="d33aa-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d33aa-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="d33aa-114">notifyDownload</span></span>|<span data-ttu-id="d33aa-115">1</span><span class="sxs-lookup"><span data-stu-id="d33aa-115">1</span></span>|<span data-ttu-id="d33aa-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="d33aa-116">Notify on download.</span></span>|
|<span data-ttu-id="d33aa-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d33aa-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="d33aa-118">duas</span><span class="sxs-lookup"><span data-stu-id="d33aa-118">2</span></span>|<span data-ttu-id="d33aa-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="d33aa-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="d33aa-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d33aa-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="d33aa-121">3D</span><span class="sxs-lookup"><span data-stu-id="d33aa-121">3</span></span>|<span data-ttu-id="d33aa-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="d33aa-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="d33aa-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="d33aa-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="d33aa-124">4 </span><span class="sxs-lookup"><span data-stu-id="d33aa-124">4</span></span>|<span data-ttu-id="d33aa-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="d33aa-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="d33aa-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="d33aa-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="d33aa-127">5 </span><span class="sxs-lookup"><span data-stu-id="d33aa-127">5</span></span>|<span data-ttu-id="d33aa-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="d33aa-128">Auto-install and restart without end-user control</span></span>|







