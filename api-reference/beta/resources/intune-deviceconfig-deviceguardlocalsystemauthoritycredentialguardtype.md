---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 481bcb0bfb1380017a2b9261f6896f69e78b40b6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724590"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="6467a-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="6467a-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="6467a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6467a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6467a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6467a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6467a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6467a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6467a-107">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="6467a-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="6467a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6467a-108">Members</span></span>
|<span data-ttu-id="6467a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6467a-109">Member</span></span>|<span data-ttu-id="6467a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6467a-110">Value</span></span>|<span data-ttu-id="6467a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6467a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6467a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6467a-112">notConfigured</span></span>|<span data-ttu-id="6467a-113">,0</span><span class="sxs-lookup"><span data-stu-id="6467a-113">0</span></span>|<span data-ttu-id="6467a-114">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="6467a-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="6467a-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="6467a-115">enableWithUEFILock</span></span>|<span data-ttu-id="6467a-116">1</span><span class="sxs-lookup"><span data-stu-id="6467a-116">1</span></span>|<span data-ttu-id="6467a-117">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="6467a-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="6467a-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="6467a-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="6467a-119">duas</span><span class="sxs-lookup"><span data-stu-id="6467a-119">2</span></span>|<span data-ttu-id="6467a-120">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="6467a-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="6467a-121">desabilitar</span><span class="sxs-lookup"><span data-stu-id="6467a-121">disable</span></span>|<span data-ttu-id="6467a-122">3D</span><span class="sxs-lookup"><span data-stu-id="6467a-122">3</span></span>|<span data-ttu-id="6467a-123">Desabilita a proteção de credenciais.</span><span class="sxs-lookup"><span data-stu-id="6467a-123">Disables Credential Guard.</span></span> <span data-ttu-id="6467a-124">Este é o valor padrão de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="6467a-124">This is the default OS value.</span></span>|





