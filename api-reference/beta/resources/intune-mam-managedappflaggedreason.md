---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64f78ca8a074d35687f50e232a104b87717a6462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527915"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="dc26b-103">tipo de enumeração managedAppFlaggedReason</span><span class="sxs-lookup"><span data-stu-id="dc26b-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="dc26b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dc26b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc26b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc26b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc26b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc26b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc26b-107">O motivo pelo qual um usuário foi sinalizado</span><span class="sxs-lookup"><span data-stu-id="dc26b-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="dc26b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="dc26b-108">Members</span></span>
|<span data-ttu-id="dc26b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="dc26b-109">Member</span></span>|<span data-ttu-id="dc26b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="dc26b-110">Value</span></span>|<span data-ttu-id="dc26b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc26b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc26b-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="dc26b-112">none</span></span>|<span data-ttu-id="dc26b-113">,0</span><span class="sxs-lookup"><span data-stu-id="dc26b-113">0</span></span>|<span data-ttu-id="dc26b-114">Nenhum problema.</span><span class="sxs-lookup"><span data-stu-id="dc26b-114">No issue.</span></span>|
|<span data-ttu-id="dc26b-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="dc26b-115">rootedDevice</span></span>|<span data-ttu-id="dc26b-116">1 </span><span class="sxs-lookup"><span data-stu-id="dc26b-116">1</span></span>|<span data-ttu-id="dc26b-117">O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="dc26b-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="dc26b-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="dc26b-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="dc26b-119">2 </span><span class="sxs-lookup"><span data-stu-id="dc26b-119">2</span></span>|<span data-ttu-id="dc26b-120">O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="dc26b-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="dc26b-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="dc26b-121">androidFactoryRomModified</span></span>|<span data-ttu-id="dc26b-122">3 </span><span class="sxs-lookup"><span data-stu-id="dc26b-122">3</span></span>|<span data-ttu-id="dc26b-123">O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.</span><span class="sxs-lookup"><span data-stu-id="dc26b-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



