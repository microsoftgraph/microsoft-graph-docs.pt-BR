---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90366deee96e898d8339d59cb1a49879ba019c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075900"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b794e-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="b794e-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="b794e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b794e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b794e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b794e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b794e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b794e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b794e-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="b794e-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="b794e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b794e-108">Members</span></span>
|<span data-ttu-id="b794e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b794e-109">Member</span></span>|<span data-ttu-id="b794e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b794e-110">Value</span></span>|<span data-ttu-id="b794e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b794e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b794e-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="b794e-112">userDefined</span></span>|<span data-ttu-id="b794e-113">,0</span><span class="sxs-lookup"><span data-stu-id="b794e-113">0</span></span>|<span data-ttu-id="b794e-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b794e-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b794e-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b794e-115">notifyDownload</span></span>|<span data-ttu-id="b794e-116">1 </span><span class="sxs-lookup"><span data-stu-id="b794e-116">1</span></span>|<span data-ttu-id="b794e-117">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="b794e-117">Notify on download.</span></span>|
|<span data-ttu-id="b794e-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b794e-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b794e-119">2 </span><span class="sxs-lookup"><span data-stu-id="b794e-119">2</span></span>|<span data-ttu-id="b794e-120">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b794e-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b794e-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b794e-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b794e-122">3 </span><span class="sxs-lookup"><span data-stu-id="b794e-122">3</span></span>|<span data-ttu-id="b794e-123">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b794e-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b794e-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b794e-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b794e-125">4 </span><span class="sxs-lookup"><span data-stu-id="b794e-125">4</span></span>|<span data-ttu-id="b794e-126">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="b794e-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b794e-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b794e-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b794e-128">5 </span><span class="sxs-lookup"><span data-stu-id="b794e-128">5</span></span>|<span data-ttu-id="b794e-129">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="b794e-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="b794e-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="b794e-130">windowsDefault</span></span>|<span data-ttu-id="b794e-131">6 </span><span class="sxs-lookup"><span data-stu-id="b794e-131">6</span></span>|<span data-ttu-id="b794e-132">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="b794e-132">Reset to Windows default value.</span></span>|






