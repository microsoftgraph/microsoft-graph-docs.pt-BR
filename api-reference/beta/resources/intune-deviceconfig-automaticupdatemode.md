---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d44c4db05be66f568ba5c0b9182a6d2ab509088
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527070"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="2054a-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="2054a-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="2054a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2054a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2054a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2054a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2054a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2054a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2054a-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="2054a-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="2054a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2054a-108">Members</span></span>
|<span data-ttu-id="2054a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2054a-109">Member</span></span>|<span data-ttu-id="2054a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2054a-110">Value</span></span>|<span data-ttu-id="2054a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2054a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2054a-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="2054a-112">userDefined</span></span>|<span data-ttu-id="2054a-113">,0</span><span class="sxs-lookup"><span data-stu-id="2054a-113">0</span></span>|<span data-ttu-id="2054a-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="2054a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2054a-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="2054a-115">notifyDownload</span></span>|<span data-ttu-id="2054a-116">1 </span><span class="sxs-lookup"><span data-stu-id="2054a-116">1</span></span>|<span data-ttu-id="2054a-117">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="2054a-117">Notify on download.</span></span>|
|<span data-ttu-id="2054a-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="2054a-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="2054a-119">2 </span><span class="sxs-lookup"><span data-stu-id="2054a-119">2</span></span>|<span data-ttu-id="2054a-120">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="2054a-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="2054a-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="2054a-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="2054a-122">3 </span><span class="sxs-lookup"><span data-stu-id="2054a-122">3</span></span>|<span data-ttu-id="2054a-123">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="2054a-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="2054a-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="2054a-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="2054a-125">4 </span><span class="sxs-lookup"><span data-stu-id="2054a-125">4</span></span>|<span data-ttu-id="2054a-126">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="2054a-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="2054a-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="2054a-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="2054a-128">5 </span><span class="sxs-lookup"><span data-stu-id="2054a-128">5</span></span>|<span data-ttu-id="2054a-129">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="2054a-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="2054a-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="2054a-130">windowsDefault</span></span>|<span data-ttu-id="2054a-131">6 </span><span class="sxs-lookup"><span data-stu-id="2054a-131">6</span></span>|<span data-ttu-id="2054a-132">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="2054a-132">Reset to Windows default value.</span></span>|



