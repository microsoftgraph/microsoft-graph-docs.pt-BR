---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d0723bef94d187452d6b622c290f7e4cb0182db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532614"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="07f94-103">tipo de enumeração Propriedades automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="07f94-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="07f94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07f94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f94-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="07f94-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="07f94-107">Membros</span><span class="sxs-lookup"><span data-stu-id="07f94-107">Members</span></span>
|<span data-ttu-id="07f94-108">Membro</span><span class="sxs-lookup"><span data-stu-id="07f94-108">Member</span></span>|<span data-ttu-id="07f94-109">Valor</span><span class="sxs-lookup"><span data-stu-id="07f94-109">Value</span></span>|<span data-ttu-id="07f94-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07f94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f94-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="07f94-111">userDefined</span></span>|<span data-ttu-id="07f94-112">,0</span><span class="sxs-lookup"><span data-stu-id="07f94-112">0</span></span>|<span data-ttu-id="07f94-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="07f94-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="07f94-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="07f94-114">notifyDownload</span></span>|<span data-ttu-id="07f94-115">1 </span><span class="sxs-lookup"><span data-stu-id="07f94-115">1</span></span>|<span data-ttu-id="07f94-116">Notifique o download.</span><span class="sxs-lookup"><span data-stu-id="07f94-116">Notify on download.</span></span>|
|<span data-ttu-id="07f94-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="07f94-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="07f94-118">2 </span><span class="sxs-lookup"><span data-stu-id="07f94-118">2</span></span>|<span data-ttu-id="07f94-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="07f94-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="07f94-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="07f94-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="07f94-121">3 </span><span class="sxs-lookup"><span data-stu-id="07f94-121">3</span></span>|<span data-ttu-id="07f94-122">Instalação automática e reinicialização no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="07f94-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="07f94-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="07f94-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="07f94-124">4 </span><span class="sxs-lookup"><span data-stu-id="07f94-124">4</span></span>|<span data-ttu-id="07f94-125">Instalação automática e reinicialização no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="07f94-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="07f94-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="07f94-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="07f94-127">5 </span><span class="sxs-lookup"><span data-stu-id="07f94-127">5</span></span>|<span data-ttu-id="07f94-128">Instalação e reinício automáticos sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="07f94-128">Auto-install and restart without end-user control</span></span>|




