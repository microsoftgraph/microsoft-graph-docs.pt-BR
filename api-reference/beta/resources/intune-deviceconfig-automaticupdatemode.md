---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549335"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b564e-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="b564e-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="b564e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b564e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b564e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b564e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b564e-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="b564e-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="b564e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b564e-107">Members</span></span>
|<span data-ttu-id="b564e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b564e-108">Member</span></span>|<span data-ttu-id="b564e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b564e-109">Value</span></span>|<span data-ttu-id="b564e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b564e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b564e-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="b564e-111">userDefined</span></span>|<span data-ttu-id="b564e-112">,0</span><span class="sxs-lookup"><span data-stu-id="b564e-112">0</span></span>|<span data-ttu-id="b564e-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b564e-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b564e-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b564e-114">notifyDownload</span></span>|<span data-ttu-id="b564e-115">1 </span><span class="sxs-lookup"><span data-stu-id="b564e-115">1</span></span>|<span data-ttu-id="b564e-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="b564e-116">Notify on download.</span></span>|
|<span data-ttu-id="b564e-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b564e-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b564e-118">2 </span><span class="sxs-lookup"><span data-stu-id="b564e-118">2</span></span>|<span data-ttu-id="b564e-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b564e-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b564e-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b564e-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b564e-121">3 </span><span class="sxs-lookup"><span data-stu-id="b564e-121">3</span></span>|<span data-ttu-id="b564e-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b564e-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b564e-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b564e-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b564e-124">4 </span><span class="sxs-lookup"><span data-stu-id="b564e-124">4</span></span>|<span data-ttu-id="b564e-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="b564e-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b564e-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b564e-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b564e-127">5 </span><span class="sxs-lookup"><span data-stu-id="b564e-127">5</span></span>|<span data-ttu-id="b564e-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="b564e-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="b564e-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="b564e-129">windowsDefault</span></span>|<span data-ttu-id="b564e-130">6 </span><span class="sxs-lookup"><span data-stu-id="b564e-130">6</span></span>|<span data-ttu-id="b564e-131">ReDefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="b564e-131">Reset to Windows default value.</span></span>|





