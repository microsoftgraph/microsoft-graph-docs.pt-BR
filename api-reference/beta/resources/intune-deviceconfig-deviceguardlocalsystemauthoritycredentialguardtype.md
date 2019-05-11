---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 284f0fd4256a3e7f70cc463eecd6ca9655c7ec04
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947012"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="a9f7a-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="a9f7a-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="a9f7a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f7a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f7a-106">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="a9f7a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a9f7a-107">Members</span></span>
|<span data-ttu-id="a9f7a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a9f7a-108">Member</span></span>|<span data-ttu-id="a9f7a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a9f7a-109">Value</span></span>|<span data-ttu-id="a9f7a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9f7a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f7a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a9f7a-111">notConfigured</span></span>|<span data-ttu-id="a9f7a-112">,0</span><span class="sxs-lookup"><span data-stu-id="a9f7a-112">0</span></span>|<span data-ttu-id="a9f7a-113">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="a9f7a-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="a9f7a-114">enableWithUEFILock</span></span>|<span data-ttu-id="a9f7a-115">1</span><span class="sxs-lookup"><span data-stu-id="a9f7a-115">1</span></span>|<span data-ttu-id="a9f7a-116">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="a9f7a-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="a9f7a-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="a9f7a-118">duas</span><span class="sxs-lookup"><span data-stu-id="a9f7a-118">2</span></span>|<span data-ttu-id="a9f7a-119">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a9f7a-119">Turns on Credential Guard without UEFI lock.</span></span>|




