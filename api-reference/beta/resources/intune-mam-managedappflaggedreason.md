---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 08d21f78466f7f716b5d9bffcd1832e5c1a23d89
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259680"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="1d593-103">tipo de enumeração managedAppFlaggedReason</span><span class="sxs-lookup"><span data-stu-id="1d593-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="1d593-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d593-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d593-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d593-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d593-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d593-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d593-107">O motivo pelo qual um usuário foi sinalizado</span><span class="sxs-lookup"><span data-stu-id="1d593-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="1d593-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1d593-108">Members</span></span>
|<span data-ttu-id="1d593-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1d593-109">Member</span></span>|<span data-ttu-id="1d593-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1d593-110">Value</span></span>|<span data-ttu-id="1d593-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d593-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d593-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="1d593-112">none</span></span>|<span data-ttu-id="1d593-113">,0</span><span class="sxs-lookup"><span data-stu-id="1d593-113">0</span></span>|<span data-ttu-id="1d593-114">Nenhum problema.</span><span class="sxs-lookup"><span data-stu-id="1d593-114">No issue.</span></span>|
|<span data-ttu-id="1d593-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="1d593-115">rootedDevice</span></span>|<span data-ttu-id="1d593-116">1</span><span class="sxs-lookup"><span data-stu-id="1d593-116">1</span></span>|<span data-ttu-id="1d593-117">O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d593-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="1d593-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="1d593-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="1d593-119">duas</span><span class="sxs-lookup"><span data-stu-id="1d593-119">2</span></span>|<span data-ttu-id="1d593-120">O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d593-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="1d593-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="1d593-121">androidFactoryRomModified</span></span>|<span data-ttu-id="1d593-122">3D</span><span class="sxs-lookup"><span data-stu-id="1d593-122">3</span></span>|<span data-ttu-id="1d593-123">O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1d593-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




