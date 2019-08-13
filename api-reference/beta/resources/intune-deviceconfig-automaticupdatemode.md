---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8d64f3af656a03bd02ecba5db2fbdab288f3693
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333881"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="65e77-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="65e77-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="65e77-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65e77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65e77-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65e77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e77-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="65e77-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="65e77-107">Membros</span><span class="sxs-lookup"><span data-stu-id="65e77-107">Members</span></span>
|<span data-ttu-id="65e77-108">Membro</span><span class="sxs-lookup"><span data-stu-id="65e77-108">Member</span></span>|<span data-ttu-id="65e77-109">Valor</span><span class="sxs-lookup"><span data-stu-id="65e77-109">Value</span></span>|<span data-ttu-id="65e77-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65e77-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e77-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="65e77-111">userDefined</span></span>|<span data-ttu-id="65e77-112">,0</span><span class="sxs-lookup"><span data-stu-id="65e77-112">0</span></span>|<span data-ttu-id="65e77-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="65e77-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="65e77-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="65e77-114">notifyDownload</span></span>|<span data-ttu-id="65e77-115">1</span><span class="sxs-lookup"><span data-stu-id="65e77-115">1</span></span>|<span data-ttu-id="65e77-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="65e77-116">Notify on download.</span></span>|
|<span data-ttu-id="65e77-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="65e77-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="65e77-118">duas</span><span class="sxs-lookup"><span data-stu-id="65e77-118">2</span></span>|<span data-ttu-id="65e77-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="65e77-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="65e77-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="65e77-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="65e77-121">3D</span><span class="sxs-lookup"><span data-stu-id="65e77-121">3</span></span>|<span data-ttu-id="65e77-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="65e77-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="65e77-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="65e77-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="65e77-124">quatro</span><span class="sxs-lookup"><span data-stu-id="65e77-124">4</span></span>|<span data-ttu-id="65e77-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="65e77-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="65e77-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="65e77-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="65e77-127">0,5</span><span class="sxs-lookup"><span data-stu-id="65e77-127">5</span></span>|<span data-ttu-id="65e77-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="65e77-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="65e77-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="65e77-129">windowsDefault</span></span>|<span data-ttu-id="65e77-130">6</span><span class="sxs-lookup"><span data-stu-id="65e77-130">6</span></span>|<span data-ttu-id="65e77-131">Redefina como o valor padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="65e77-131">Reset to Windows default value.</span></span>|



