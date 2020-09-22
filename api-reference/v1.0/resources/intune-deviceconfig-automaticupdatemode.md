---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e02f1a3ed99840382148d4f1434df667e2391739
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051113"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b745d-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="b745d-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="b745d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b745d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b745d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b745d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b745d-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="b745d-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="b745d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b745d-107">Members</span></span>
|<span data-ttu-id="b745d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b745d-108">Member</span></span>|<span data-ttu-id="b745d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b745d-109">Value</span></span>|<span data-ttu-id="b745d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b745d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b745d-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="b745d-111">userDefined</span></span>|<span data-ttu-id="b745d-112">,0</span><span class="sxs-lookup"><span data-stu-id="b745d-112">0</span></span>|<span data-ttu-id="b745d-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b745d-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b745d-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b745d-114">notifyDownload</span></span>|<span data-ttu-id="b745d-115">1 </span><span class="sxs-lookup"><span data-stu-id="b745d-115">1</span></span>|<span data-ttu-id="b745d-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="b745d-116">Notify on download.</span></span>|
|<span data-ttu-id="b745d-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b745d-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b745d-118">2 </span><span class="sxs-lookup"><span data-stu-id="b745d-118">2</span></span>|<span data-ttu-id="b745d-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b745d-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b745d-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b745d-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b745d-121">3 </span><span class="sxs-lookup"><span data-stu-id="b745d-121">3</span></span>|<span data-ttu-id="b745d-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="b745d-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b745d-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b745d-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b745d-124">4 </span><span class="sxs-lookup"><span data-stu-id="b745d-124">4</span></span>|<span data-ttu-id="b745d-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="b745d-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b745d-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b745d-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b745d-127">5 </span><span class="sxs-lookup"><span data-stu-id="b745d-127">5</span></span>|<span data-ttu-id="b745d-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="b745d-128">Auto-install and restart without end-user control</span></span>|









