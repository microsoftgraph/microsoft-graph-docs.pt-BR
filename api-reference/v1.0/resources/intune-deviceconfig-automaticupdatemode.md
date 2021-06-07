---
title: Tipo de número automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b4cd222db425a9a8a2647f2ffbeb6056dddbe1c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755900"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="26acc-103">Tipo de número automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="26acc-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="26acc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26acc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26acc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26acc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26acc-106">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="26acc-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="26acc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="26acc-107">Members</span></span>
|<span data-ttu-id="26acc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="26acc-108">Member</span></span>|<span data-ttu-id="26acc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="26acc-109">Value</span></span>|<span data-ttu-id="26acc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26acc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26acc-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="26acc-111">userDefined</span></span>|<span data-ttu-id="26acc-112">0</span><span class="sxs-lookup"><span data-stu-id="26acc-112">0</span></span>|<span data-ttu-id="26acc-113">User Defined, default value, no intent.</span><span class="sxs-lookup"><span data-stu-id="26acc-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="26acc-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="26acc-114">notifyDownload</span></span>|<span data-ttu-id="26acc-115">1</span><span class="sxs-lookup"><span data-stu-id="26acc-115">1</span></span>|<span data-ttu-id="26acc-116">Notificar no download.</span><span class="sxs-lookup"><span data-stu-id="26acc-116">Notify on download.</span></span>|
|<span data-ttu-id="26acc-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="26acc-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="26acc-118">2</span><span class="sxs-lookup"><span data-stu-id="26acc-118">2</span></span>|<span data-ttu-id="26acc-119">Instalação automática no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="26acc-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="26acc-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="26acc-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="26acc-121">3</span><span class="sxs-lookup"><span data-stu-id="26acc-121">3</span></span>|<span data-ttu-id="26acc-122">Instale e reinicie automaticamente no momento da manutenção.</span><span class="sxs-lookup"><span data-stu-id="26acc-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="26acc-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="26acc-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="26acc-124">4 </span><span class="sxs-lookup"><span data-stu-id="26acc-124">4</span></span>|<span data-ttu-id="26acc-125">Instale e reinicie automaticamente no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="26acc-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="26acc-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="26acc-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="26acc-127">5 </span><span class="sxs-lookup"><span data-stu-id="26acc-127">5</span></span>|<span data-ttu-id="26acc-128">Instalar e reiniciar automaticamente sem o controle do usuário final</span><span class="sxs-lookup"><span data-stu-id="26acc-128">Auto-install and restart without end-user control</span></span>|




