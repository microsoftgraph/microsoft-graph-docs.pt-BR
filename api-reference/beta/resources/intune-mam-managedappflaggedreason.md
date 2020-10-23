---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bfe1ee2fe8385150336bef52ba2e498832b60562
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684537"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="349d3-103">tipo de enumeração managedAppFlaggedReason</span><span class="sxs-lookup"><span data-stu-id="349d3-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="349d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="349d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="349d3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="349d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="349d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="349d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="349d3-107">O motivo pelo qual um usuário foi sinalizado</span><span class="sxs-lookup"><span data-stu-id="349d3-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="349d3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="349d3-108">Members</span></span>
|<span data-ttu-id="349d3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="349d3-109">Member</span></span>|<span data-ttu-id="349d3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="349d3-110">Value</span></span>|<span data-ttu-id="349d3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="349d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="349d3-112">none</span><span class="sxs-lookup"><span data-stu-id="349d3-112">none</span></span>|<span data-ttu-id="349d3-113">,0</span><span class="sxs-lookup"><span data-stu-id="349d3-113">0</span></span>|<span data-ttu-id="349d3-114">Nenhum problema.</span><span class="sxs-lookup"><span data-stu-id="349d3-114">No issue.</span></span>|
|<span data-ttu-id="349d3-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="349d3-115">rootedDevice</span></span>|<span data-ttu-id="349d3-116">1</span><span class="sxs-lookup"><span data-stu-id="349d3-116">1</span></span>|<span data-ttu-id="349d3-117">O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="349d3-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="349d3-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="349d3-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="349d3-119">duas</span><span class="sxs-lookup"><span data-stu-id="349d3-119">2</span></span>|<span data-ttu-id="349d3-120">O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="349d3-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="349d3-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="349d3-121">androidFactoryRomModified</span></span>|<span data-ttu-id="349d3-122">3D</span><span class="sxs-lookup"><span data-stu-id="349d3-122">3</span></span>|<span data-ttu-id="349d3-123">O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.</span><span class="sxs-lookup"><span data-stu-id="349d3-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





