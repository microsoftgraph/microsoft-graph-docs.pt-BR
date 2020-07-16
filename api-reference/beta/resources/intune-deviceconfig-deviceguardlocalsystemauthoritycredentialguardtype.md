---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b02402ff6c6c0373396bd6fca0cad6ded5cb36d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123768"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="a61f0-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="a61f0-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="a61f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a61f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a61f0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a61f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a61f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a61f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a61f0-107">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="a61f0-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="a61f0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a61f0-108">Members</span></span>
|<span data-ttu-id="a61f0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a61f0-109">Member</span></span>|<span data-ttu-id="a61f0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a61f0-110">Value</span></span>|<span data-ttu-id="a61f0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a61f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a61f0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a61f0-112">notConfigured</span></span>|<span data-ttu-id="a61f0-113">,0</span><span class="sxs-lookup"><span data-stu-id="a61f0-113">0</span></span>|<span data-ttu-id="a61f0-114">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a61f0-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="a61f0-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="a61f0-115">enableWithUEFILock</span></span>|<span data-ttu-id="a61f0-116">1 </span><span class="sxs-lookup"><span data-stu-id="a61f0-116">1</span></span>|<span data-ttu-id="a61f0-117">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a61f0-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="a61f0-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="a61f0-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="a61f0-119">2 </span><span class="sxs-lookup"><span data-stu-id="a61f0-119">2</span></span>|<span data-ttu-id="a61f0-120">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="a61f0-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="a61f0-121">desabilitar</span><span class="sxs-lookup"><span data-stu-id="a61f0-121">disable</span></span>|<span data-ttu-id="a61f0-122">3 </span><span class="sxs-lookup"><span data-stu-id="a61f0-122">3</span></span>|<span data-ttu-id="a61f0-123">Desabilita a proteção de credenciais.</span><span class="sxs-lookup"><span data-stu-id="a61f0-123">Disables Credential Guard.</span></span> <span data-ttu-id="a61f0-124">Este é o valor padrão de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="a61f0-124">This is the default OS value.</span></span>|



