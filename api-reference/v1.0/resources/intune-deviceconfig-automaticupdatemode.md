---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a0cc2d3918573fca6480c6eecd07889534cda4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028571"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="06c25-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="06c25-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="06c25-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06c25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c25-105">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="06c25-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="06c25-106">Membros</span><span class="sxs-lookup"><span data-stu-id="06c25-106">Members</span></span>
|<span data-ttu-id="06c25-107">Membro</span><span class="sxs-lookup"><span data-stu-id="06c25-107">Member</span></span>|<span data-ttu-id="06c25-108">Valor</span><span class="sxs-lookup"><span data-stu-id="06c25-108">Value</span></span>|<span data-ttu-id="06c25-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="06c25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c25-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="06c25-110">userDefined</span></span>|<span data-ttu-id="06c25-111">,0</span><span class="sxs-lookup"><span data-stu-id="06c25-111">0</span></span>|<span data-ttu-id="06c25-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="06c25-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="06c25-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="06c25-113">notifyDownload</span></span>|<span data-ttu-id="06c25-114">1</span><span class="sxs-lookup"><span data-stu-id="06c25-114">1</span></span>|<span data-ttu-id="06c25-115">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="06c25-115">Notify on download.</span></span>|
|<span data-ttu-id="06c25-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="06c25-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="06c25-117">duas</span><span class="sxs-lookup"><span data-stu-id="06c25-117">2</span></span>|<span data-ttu-id="06c25-118">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="06c25-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="06c25-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="06c25-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="06c25-120">3D</span><span class="sxs-lookup"><span data-stu-id="06c25-120">3</span></span>|<span data-ttu-id="06c25-121">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="06c25-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="06c25-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="06c25-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="06c25-123">quatro</span><span class="sxs-lookup"><span data-stu-id="06c25-123">4</span></span>|<span data-ttu-id="06c25-124">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="06c25-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="06c25-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="06c25-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="06c25-126">0,5</span><span class="sxs-lookup"><span data-stu-id="06c25-126">5</span></span>|<span data-ttu-id="06c25-127">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="06c25-127">Auto-install and restart without end-user control</span></span>|



