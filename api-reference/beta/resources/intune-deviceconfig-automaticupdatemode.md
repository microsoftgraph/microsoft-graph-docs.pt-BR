---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913265"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c25bb-103">tipo de enum automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="c25bb-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="c25bb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c25bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c25bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c25bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c25bb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c25bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c25bb-107">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="c25bb-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="c25bb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c25bb-108">Members</span></span>
|<span data-ttu-id="c25bb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c25bb-109">Member</span></span>|<span data-ttu-id="c25bb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c25bb-110">Value</span></span>|<span data-ttu-id="c25bb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c25bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c25bb-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="c25bb-112">userDefined</span></span>|<span data-ttu-id="c25bb-113">0</span><span class="sxs-lookup"><span data-stu-id="c25bb-113">0</span></span>|<span data-ttu-id="c25bb-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c25bb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c25bb-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="c25bb-115">notifyDownload</span></span>|<span data-ttu-id="c25bb-116">1</span><span class="sxs-lookup"><span data-stu-id="c25bb-116">1</span></span>|<span data-ttu-id="c25bb-117">Notifica baixados.</span><span class="sxs-lookup"><span data-stu-id="c25bb-117">Notify on download.</span></span>|
|<span data-ttu-id="c25bb-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c25bb-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c25bb-119">2</span><span class="sxs-lookup"><span data-stu-id="c25bb-119">2</span></span>|<span data-ttu-id="c25bb-120">Instalar automaticamente em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="c25bb-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c25bb-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c25bb-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c25bb-122">3</span><span class="sxs-lookup"><span data-stu-id="c25bb-122">3</span></span>|<span data-ttu-id="c25bb-123">Instalar automaticamente e reinicialize em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="c25bb-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c25bb-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c25bb-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c25bb-125">4</span><span class="sxs-lookup"><span data-stu-id="c25bb-125">4</span></span>|<span data-ttu-id="c25bb-126">Instalar automaticamente e reinicialize no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="c25bb-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c25bb-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c25bb-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c25bb-128">5</span><span class="sxs-lookup"><span data-stu-id="c25bb-128">5</span></span>|<span data-ttu-id="c25bb-129">Instalar automaticamente e reinicie sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="c25bb-129">Auto-install and restart without end-user control</span></span>|





