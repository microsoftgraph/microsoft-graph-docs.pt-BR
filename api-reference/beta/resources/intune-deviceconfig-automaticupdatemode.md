---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2fffa3e1b1a5e7efa43d7ce653792247e3ad790
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983628"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="4cb97-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="4cb97-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="4cb97-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4cb97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cb97-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4cb97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cb97-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="4cb97-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="4cb97-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4cb97-107">Members</span></span>
|<span data-ttu-id="4cb97-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4cb97-108">Member</span></span>|<span data-ttu-id="4cb97-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4cb97-109">Value</span></span>|<span data-ttu-id="4cb97-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cb97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb97-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="4cb97-111">userDefined</span></span>|<span data-ttu-id="4cb97-112">,0</span><span class="sxs-lookup"><span data-stu-id="4cb97-112">0</span></span>|<span data-ttu-id="4cb97-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="4cb97-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="4cb97-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="4cb97-114">notifyDownload</span></span>|<span data-ttu-id="4cb97-115">1</span><span class="sxs-lookup"><span data-stu-id="4cb97-115">1</span></span>|<span data-ttu-id="4cb97-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="4cb97-116">Notify on download.</span></span>|
|<span data-ttu-id="4cb97-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="4cb97-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="4cb97-118">duas</span><span class="sxs-lookup"><span data-stu-id="4cb97-118">2</span></span>|<span data-ttu-id="4cb97-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="4cb97-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="4cb97-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="4cb97-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="4cb97-121">3D</span><span class="sxs-lookup"><span data-stu-id="4cb97-121">3</span></span>|<span data-ttu-id="4cb97-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="4cb97-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="4cb97-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="4cb97-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="4cb97-124">quatro</span><span class="sxs-lookup"><span data-stu-id="4cb97-124">4</span></span>|<span data-ttu-id="4cb97-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="4cb97-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="4cb97-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="4cb97-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="4cb97-127">0,5</span><span class="sxs-lookup"><span data-stu-id="4cb97-127">5</span></span>|<span data-ttu-id="4cb97-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="4cb97-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="4cb97-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="4cb97-129">windowsDefault</span></span>|<span data-ttu-id="4cb97-130">6</span><span class="sxs-lookup"><span data-stu-id="4cb97-130">6</span></span>|<span data-ttu-id="4cb97-131">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="4cb97-131">Reset to Windows default value.</span></span>|





