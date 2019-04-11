---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf3190ce35d56ef83d19368001175896cb794c01
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772367"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="f4fa4-103">tipo de enumeração managedAppFlaggedReason</span><span class="sxs-lookup"><span data-stu-id="f4fa4-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="f4fa4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4fa4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4fa4-106">O motivo pelo qual um usuário foi sinalizado</span><span class="sxs-lookup"><span data-stu-id="f4fa4-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="f4fa4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f4fa4-107">Members</span></span>
|<span data-ttu-id="f4fa4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f4fa4-108">Member</span></span>|<span data-ttu-id="f4fa4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f4fa4-109">Value</span></span>|<span data-ttu-id="f4fa4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fa4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4fa4-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="f4fa4-111">none</span></span>|<span data-ttu-id="f4fa4-112">,0</span><span class="sxs-lookup"><span data-stu-id="f4fa4-112">0</span></span>|<span data-ttu-id="f4fa4-113">Nenhum problema.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-113">No issue.</span></span>|
|<span data-ttu-id="f4fa4-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="f4fa4-114">rootedDevice</span></span>|<span data-ttu-id="f4fa4-115">1</span><span class="sxs-lookup"><span data-stu-id="f4fa4-115">1</span></span>|<span data-ttu-id="f4fa4-116">O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="f4fa4-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="f4fa4-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="f4fa4-118">duas</span><span class="sxs-lookup"><span data-stu-id="f4fa4-118">2</span></span>|<span data-ttu-id="f4fa4-119">O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="f4fa4-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="f4fa4-120">androidFactoryRomModified</span></span>|<span data-ttu-id="f4fa4-121">3D</span><span class="sxs-lookup"><span data-stu-id="f4fa4-121">3</span></span>|<span data-ttu-id="f4fa4-122">O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.</span><span class="sxs-lookup"><span data-stu-id="f4fa4-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





