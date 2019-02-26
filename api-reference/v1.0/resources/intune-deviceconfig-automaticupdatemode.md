---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251374"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="a20ab-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="a20ab-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="a20ab-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a20ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a20ab-105">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="a20ab-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="a20ab-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a20ab-106">Members</span></span>
|<span data-ttu-id="a20ab-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a20ab-107">Member</span></span>|<span data-ttu-id="a20ab-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a20ab-108">Value</span></span>|<span data-ttu-id="a20ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a20ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20ab-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="a20ab-110">userDefined</span></span>|<span data-ttu-id="a20ab-111">,0</span><span class="sxs-lookup"><span data-stu-id="a20ab-111">0</span></span>|<span data-ttu-id="a20ab-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a20ab-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a20ab-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="a20ab-113">notifyDownload</span></span>|<span data-ttu-id="a20ab-114">1</span><span class="sxs-lookup"><span data-stu-id="a20ab-114">1</span></span>|<span data-ttu-id="a20ab-115">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="a20ab-115">Notify on download.</span></span>|
|<span data-ttu-id="a20ab-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="a20ab-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="a20ab-117">duas</span><span class="sxs-lookup"><span data-stu-id="a20ab-117">2</span></span>|<span data-ttu-id="a20ab-118">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="a20ab-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="a20ab-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="a20ab-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="a20ab-120">3D</span><span class="sxs-lookup"><span data-stu-id="a20ab-120">3</span></span>|<span data-ttu-id="a20ab-121">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="a20ab-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="a20ab-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="a20ab-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="a20ab-123">quatro</span><span class="sxs-lookup"><span data-stu-id="a20ab-123">4</span></span>|<span data-ttu-id="a20ab-124">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="a20ab-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="a20ab-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="a20ab-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="a20ab-126">0,5</span><span class="sxs-lookup"><span data-stu-id="a20ab-126">5</span></span>|<span data-ttu-id="a20ab-127">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="a20ab-127">Auto-install and restart without end-user control</span></span>|



