---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402633"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="18e78-103">tipo de enum automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="18e78-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="18e78-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="18e78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18e78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18e78-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="18e78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18e78-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="18e78-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="18e78-108">Membros</span><span class="sxs-lookup"><span data-stu-id="18e78-108">Members</span></span>
|<span data-ttu-id="18e78-109">Membro</span><span class="sxs-lookup"><span data-stu-id="18e78-109">Member</span></span>|<span data-ttu-id="18e78-110">Valor</span><span class="sxs-lookup"><span data-stu-id="18e78-110">Value</span></span>|<span data-ttu-id="18e78-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18e78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e78-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="18e78-112">userDefined</span></span>|<span data-ttu-id="18e78-113">0</span><span class="sxs-lookup"><span data-stu-id="18e78-113">0</span></span>|<span data-ttu-id="18e78-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="18e78-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="18e78-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="18e78-115">notifyDownload</span></span>|<span data-ttu-id="18e78-116">1</span><span class="sxs-lookup"><span data-stu-id="18e78-116">1</span></span>|<span data-ttu-id="18e78-117">Notifica baixados.</span><span class="sxs-lookup"><span data-stu-id="18e78-117">Notify on download.</span></span>|
|<span data-ttu-id="18e78-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="18e78-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="18e78-119">2</span><span class="sxs-lookup"><span data-stu-id="18e78-119">2</span></span>|<span data-ttu-id="18e78-120">Instalar automaticamente em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="18e78-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="18e78-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="18e78-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="18e78-122">3</span><span class="sxs-lookup"><span data-stu-id="18e78-122">3</span></span>|<span data-ttu-id="18e78-123">Instalar automaticamente e reinicialize em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="18e78-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="18e78-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="18e78-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="18e78-125">4</span><span class="sxs-lookup"><span data-stu-id="18e78-125">4</span></span>|<span data-ttu-id="18e78-126">Instalar automaticamente e reinicialize no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="18e78-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="18e78-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="18e78-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="18e78-128">5</span><span class="sxs-lookup"><span data-stu-id="18e78-128">5</span></span>|<span data-ttu-id="18e78-129">Instalar automaticamente e reinicie sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="18e78-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="18e78-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="18e78-130">windowsDefault</span></span>|<span data-ttu-id="18e78-131">6</span><span class="sxs-lookup"><span data-stu-id="18e78-131">6</span></span>|<span data-ttu-id="18e78-132">Redefinido para o valor de padrão do Windows.</span><span class="sxs-lookup"><span data-stu-id="18e78-132">Reset to Windows default value.</span></span>|




