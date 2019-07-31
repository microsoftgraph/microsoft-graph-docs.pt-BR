---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d5df7cc791947e46b5da11c3162c0c5cf945bdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011467"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="bacf4-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="bacf4-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="bacf4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bacf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bacf4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bacf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacf4-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="bacf4-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="bacf4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bacf4-107">Members</span></span>
|<span data-ttu-id="bacf4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bacf4-108">Member</span></span>|<span data-ttu-id="bacf4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bacf4-109">Value</span></span>|<span data-ttu-id="bacf4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacf4-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="bacf4-111">userDefined</span></span>|<span data-ttu-id="bacf4-112">,0</span><span class="sxs-lookup"><span data-stu-id="bacf4-112">0</span></span>|<span data-ttu-id="bacf4-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="bacf4-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="bacf4-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="bacf4-114">notifyDownload</span></span>|<span data-ttu-id="bacf4-115">1</span><span class="sxs-lookup"><span data-stu-id="bacf4-115">1</span></span>|<span data-ttu-id="bacf4-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="bacf4-116">Notify on download.</span></span>|
|<span data-ttu-id="bacf4-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="bacf4-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="bacf4-118">duas</span><span class="sxs-lookup"><span data-stu-id="bacf4-118">2</span></span>|<span data-ttu-id="bacf4-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="bacf4-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="bacf4-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="bacf4-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="bacf4-121">3D</span><span class="sxs-lookup"><span data-stu-id="bacf4-121">3</span></span>|<span data-ttu-id="bacf4-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="bacf4-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="bacf4-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="bacf4-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="bacf4-124">quatro</span><span class="sxs-lookup"><span data-stu-id="bacf4-124">4</span></span>|<span data-ttu-id="bacf4-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="bacf4-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="bacf4-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="bacf4-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="bacf4-127">0,5</span><span class="sxs-lookup"><span data-stu-id="bacf4-127">5</span></span>|<span data-ttu-id="bacf4-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="bacf4-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="bacf4-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="bacf4-129">windowsDefault</span></span>|<span data-ttu-id="bacf4-130">6</span><span class="sxs-lookup"><span data-stu-id="bacf4-130">6</span></span>|<span data-ttu-id="bacf4-131">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="bacf4-131">Reset to Windows default value.</span></span>|





