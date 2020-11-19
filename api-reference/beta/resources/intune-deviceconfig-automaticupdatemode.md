---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a1ea942a2418f763a6914329dabe26cd0ace1e8a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260758"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="dbf59-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="dbf59-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="dbf59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbf59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbf59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbf59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbf59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbf59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf59-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="dbf59-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="dbf59-108">Membros</span><span class="sxs-lookup"><span data-stu-id="dbf59-108">Members</span></span>
|<span data-ttu-id="dbf59-109">Membro</span><span class="sxs-lookup"><span data-stu-id="dbf59-109">Member</span></span>|<span data-ttu-id="dbf59-110">Valor</span><span class="sxs-lookup"><span data-stu-id="dbf59-110">Value</span></span>|<span data-ttu-id="dbf59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbf59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf59-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="dbf59-112">userDefined</span></span>|<span data-ttu-id="dbf59-113">,0</span><span class="sxs-lookup"><span data-stu-id="dbf59-113">0</span></span>|<span data-ttu-id="dbf59-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="dbf59-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="dbf59-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="dbf59-115">notifyDownload</span></span>|<span data-ttu-id="dbf59-116">1</span><span class="sxs-lookup"><span data-stu-id="dbf59-116">1</span></span>|<span data-ttu-id="dbf59-117">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="dbf59-117">Notify on download.</span></span>|
|<span data-ttu-id="dbf59-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="dbf59-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="dbf59-119">duas</span><span class="sxs-lookup"><span data-stu-id="dbf59-119">2</span></span>|<span data-ttu-id="dbf59-120">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="dbf59-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="dbf59-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="dbf59-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="dbf59-122">3D</span><span class="sxs-lookup"><span data-stu-id="dbf59-122">3</span></span>|<span data-ttu-id="dbf59-123">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="dbf59-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="dbf59-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="dbf59-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="dbf59-125">4 </span><span class="sxs-lookup"><span data-stu-id="dbf59-125">4</span></span>|<span data-ttu-id="dbf59-126">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="dbf59-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="dbf59-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="dbf59-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="dbf59-128">5 </span><span class="sxs-lookup"><span data-stu-id="dbf59-128">5</span></span>|<span data-ttu-id="dbf59-129">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="dbf59-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="dbf59-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="dbf59-130">windowsDefault</span></span>|<span data-ttu-id="dbf59-131">6 </span><span class="sxs-lookup"><span data-stu-id="dbf59-131">6</span></span>|<span data-ttu-id="dbf59-132">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="dbf59-132">Reset to Windows default value.</span></span>|




