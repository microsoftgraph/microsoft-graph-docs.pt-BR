---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4d063858501bb8741000234bde8ade8d33550c9f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359738"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="c1c6d-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="c1c6d-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="c1c6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1c6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1c6d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1c6d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c6d-107">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="c1c6d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c1c6d-108">Members</span></span>
|<span data-ttu-id="c1c6d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c1c6d-109">Member</span></span>|<span data-ttu-id="c1c6d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c1c6d-110">Value</span></span>|<span data-ttu-id="c1c6d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c6d-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c1c6d-112">notConfigured</span></span>|<span data-ttu-id="c1c6d-113">,0</span><span class="sxs-lookup"><span data-stu-id="c1c6d-113">0</span></span>|<span data-ttu-id="c1c6d-114">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="c1c6d-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="c1c6d-115">enableWithUEFILock</span></span>|<span data-ttu-id="c1c6d-116">1</span><span class="sxs-lookup"><span data-stu-id="c1c6d-116">1</span></span>|<span data-ttu-id="c1c6d-117">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="c1c6d-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="c1c6d-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="c1c6d-119">duas</span><span class="sxs-lookup"><span data-stu-id="c1c6d-119">2</span></span>|<span data-ttu-id="c1c6d-120">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="c1c6d-120">Turns on Credential Guard without UEFI lock.</span></span>|



