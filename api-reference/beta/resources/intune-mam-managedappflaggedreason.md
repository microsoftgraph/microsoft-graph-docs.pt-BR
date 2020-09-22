---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e84a451a17964639b495340de9416b8409b5be8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030329"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="75634-103">tipo de enumeração managedAppFlaggedReason</span><span class="sxs-lookup"><span data-stu-id="75634-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="75634-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75634-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75634-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75634-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75634-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75634-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75634-107">O motivo pelo qual um usuário foi sinalizado</span><span class="sxs-lookup"><span data-stu-id="75634-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="75634-108">Membros</span><span class="sxs-lookup"><span data-stu-id="75634-108">Members</span></span>
|<span data-ttu-id="75634-109">Membro</span><span class="sxs-lookup"><span data-stu-id="75634-109">Member</span></span>|<span data-ttu-id="75634-110">Valor</span><span class="sxs-lookup"><span data-stu-id="75634-110">Value</span></span>|<span data-ttu-id="75634-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75634-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75634-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="75634-112">none</span></span>|<span data-ttu-id="75634-113">,0</span><span class="sxs-lookup"><span data-stu-id="75634-113">0</span></span>|<span data-ttu-id="75634-114">Nenhum problema.</span><span class="sxs-lookup"><span data-stu-id="75634-114">No issue.</span></span>|
|<span data-ttu-id="75634-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="75634-115">rootedDevice</span></span>|<span data-ttu-id="75634-116">1 </span><span class="sxs-lookup"><span data-stu-id="75634-116">1</span></span>|<span data-ttu-id="75634-117">O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="75634-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="75634-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="75634-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="75634-119">2 </span><span class="sxs-lookup"><span data-stu-id="75634-119">2</span></span>|<span data-ttu-id="75634-120">O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="75634-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="75634-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="75634-121">androidFactoryRomModified</span></span>|<span data-ttu-id="75634-122">3 </span><span class="sxs-lookup"><span data-stu-id="75634-122">3</span></span>|<span data-ttu-id="75634-123">O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.</span><span class="sxs-lookup"><span data-stu-id="75634-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|






