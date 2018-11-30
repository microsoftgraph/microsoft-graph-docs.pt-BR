---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003883"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="251b2-103">tipo de enum automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="251b2-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="251b2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="251b2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="251b2-105">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="251b2-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="251b2-106">Membros</span><span class="sxs-lookup"><span data-stu-id="251b2-106">Members</span></span>
|<span data-ttu-id="251b2-107">Membro</span><span class="sxs-lookup"><span data-stu-id="251b2-107">Member</span></span>|<span data-ttu-id="251b2-108">Valor</span><span class="sxs-lookup"><span data-stu-id="251b2-108">Value</span></span>|<span data-ttu-id="251b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="251b2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="251b2-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="251b2-110">userDefined</span></span>|<span data-ttu-id="251b2-111">0</span><span class="sxs-lookup"><span data-stu-id="251b2-111">0</span></span>|<span data-ttu-id="251b2-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="251b2-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="251b2-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="251b2-113">notifyDownload</span></span>|<span data-ttu-id="251b2-114">1</span><span class="sxs-lookup"><span data-stu-id="251b2-114">1</span></span>|<span data-ttu-id="251b2-115">Notifica baixados.</span><span class="sxs-lookup"><span data-stu-id="251b2-115">Notify on download.</span></span>|
|<span data-ttu-id="251b2-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="251b2-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="251b2-117">2</span><span class="sxs-lookup"><span data-stu-id="251b2-117">2</span></span>|<span data-ttu-id="251b2-118">Instalar automaticamente em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="251b2-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="251b2-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="251b2-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="251b2-120">3</span><span class="sxs-lookup"><span data-stu-id="251b2-120">3</span></span>|<span data-ttu-id="251b2-121">Instalar automaticamente e reinicialize em tempo de manutenção.</span><span class="sxs-lookup"><span data-stu-id="251b2-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="251b2-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="251b2-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="251b2-123">4</span><span class="sxs-lookup"><span data-stu-id="251b2-123">4</span></span>|<span data-ttu-id="251b2-124">Instalar automaticamente e reinicialize no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="251b2-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="251b2-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="251b2-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="251b2-126">5</span><span class="sxs-lookup"><span data-stu-id="251b2-126">5</span></span>|<span data-ttu-id="251b2-127">Instalar automaticamente e reinicie sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="251b2-127">Auto-install and restart without end-user control</span></span>|



