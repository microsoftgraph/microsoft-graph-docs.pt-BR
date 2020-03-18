---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c9532485213c97ac500057842cdcc3e5cbb6719b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792042"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="9f3be-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="9f3be-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="9f3be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f3be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f3be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f3be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f3be-106">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="9f3be-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="9f3be-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9f3be-107">Members</span></span>
|<span data-ttu-id="9f3be-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9f3be-108">Member</span></span>|<span data-ttu-id="9f3be-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9f3be-109">Value</span></span>|<span data-ttu-id="9f3be-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f3be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3be-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9f3be-111">notConfigured</span></span>|<span data-ttu-id="9f3be-112">,0</span><span class="sxs-lookup"><span data-stu-id="9f3be-112">0</span></span>|<span data-ttu-id="9f3be-113">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="9f3be-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="9f3be-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="9f3be-114">enableWithUEFILock</span></span>|<span data-ttu-id="9f3be-115">1</span><span class="sxs-lookup"><span data-stu-id="9f3be-115">1</span></span>|<span data-ttu-id="9f3be-116">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="9f3be-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="9f3be-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="9f3be-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="9f3be-118">duas</span><span class="sxs-lookup"><span data-stu-id="9f3be-118">2</span></span>|<span data-ttu-id="9f3be-119">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="9f3be-119">Turns on Credential Guard without UEFI lock.</span></span>|



