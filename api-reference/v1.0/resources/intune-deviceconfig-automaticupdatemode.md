---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987857"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b4536-103">tipo de enum automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="b4536-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="b4536-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4536-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4536-105">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="b4536-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="b4536-106">Membros</span><span class="sxs-lookup"><span data-stu-id="b4536-106">Members</span></span>
|<span data-ttu-id="b4536-107">Membro</span><span class="sxs-lookup"><span data-stu-id="b4536-107">Member</span></span>|<span data-ttu-id="b4536-108">Valor</span><span class="sxs-lookup"><span data-stu-id="b4536-108">Value</span></span>|<span data-ttu-id="b4536-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4536-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4536-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="b4536-110">userDefined</span></span>|<span data-ttu-id="b4536-111">0</span><span class="sxs-lookup"><span data-stu-id="b4536-111">0</span></span>|<span data-ttu-id="b4536-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b4536-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b4536-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b4536-113">notifyDownload</span></span>|<span data-ttu-id="b4536-114">1</span><span class="sxs-lookup"><span data-stu-id="b4536-114">1</span></span>|<span data-ttu-id="b4536-115">Notifica baixados.</span><span class="sxs-lookup"><span data-stu-id="b4536-115">Notify on download.</span></span>|
|<span data-ttu-id="b4536-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b4536-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b4536-117">2</span><span class="sxs-lookup"><span data-stu-id="b4536-117">2</span></span>|<span data-ttu-id="b4536-118">Instalar automaticamente em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="b4536-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b4536-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b4536-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b4536-120">3</span><span class="sxs-lookup"><span data-stu-id="b4536-120">3</span></span>|<span data-ttu-id="b4536-121">Instalar automaticamente e reinicialize em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="b4536-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b4536-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b4536-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b4536-123">4</span><span class="sxs-lookup"><span data-stu-id="b4536-123">4</span></span>|<span data-ttu-id="b4536-124">Instalar automaticamente e reinicialize no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="b4536-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b4536-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b4536-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b4536-126">5</span><span class="sxs-lookup"><span data-stu-id="b4536-126">5</span></span>|<span data-ttu-id="b4536-127">Instalar automaticamente e reinicie sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="b4536-127">Auto-install and restart without end-user control</span></span>|



