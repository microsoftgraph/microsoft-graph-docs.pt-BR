---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd3b2a63fe933fcd20de4f76a0ba92e31fe75b38
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725586"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="11ed9-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="11ed9-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="11ed9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ed9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11ed9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11ed9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11ed9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11ed9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11ed9-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="11ed9-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="11ed9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="11ed9-108">Members</span></span>
|<span data-ttu-id="11ed9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="11ed9-109">Member</span></span>|<span data-ttu-id="11ed9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="11ed9-110">Value</span></span>|<span data-ttu-id="11ed9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11ed9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ed9-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="11ed9-112">userDefined</span></span>|<span data-ttu-id="11ed9-113">,0</span><span class="sxs-lookup"><span data-stu-id="11ed9-113">0</span></span>|<span data-ttu-id="11ed9-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="11ed9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="11ed9-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="11ed9-115">notifyDownload</span></span>|<span data-ttu-id="11ed9-116">1</span><span class="sxs-lookup"><span data-stu-id="11ed9-116">1</span></span>|<span data-ttu-id="11ed9-117">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="11ed9-117">Notify on download.</span></span>|
|<span data-ttu-id="11ed9-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="11ed9-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="11ed9-119">duas</span><span class="sxs-lookup"><span data-stu-id="11ed9-119">2</span></span>|<span data-ttu-id="11ed9-120">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="11ed9-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="11ed9-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="11ed9-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="11ed9-122">3D</span><span class="sxs-lookup"><span data-stu-id="11ed9-122">3</span></span>|<span data-ttu-id="11ed9-123">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="11ed9-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="11ed9-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="11ed9-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="11ed9-125">4 </span><span class="sxs-lookup"><span data-stu-id="11ed9-125">4</span></span>|<span data-ttu-id="11ed9-126">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="11ed9-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="11ed9-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="11ed9-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="11ed9-128">5 </span><span class="sxs-lookup"><span data-stu-id="11ed9-128">5</span></span>|<span data-ttu-id="11ed9-129">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="11ed9-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="11ed9-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="11ed9-130">windowsDefault</span></span>|<span data-ttu-id="11ed9-131">6 </span><span class="sxs-lookup"><span data-stu-id="11ed9-131">6</span></span>|<span data-ttu-id="11ed9-132">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="11ed9-132">Reset to Windows default value.</span></span>|





