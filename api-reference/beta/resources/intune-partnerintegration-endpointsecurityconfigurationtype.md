---
title: tipo de enumeração endpointSecurityConfigurationType
description: O tipo de política de segurança do ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5e772e9c32ad304bab3830701852b170f479cdf7
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793160"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="67b4f-103">tipo de enumeração endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="67b4f-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="67b4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67b4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67b4f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67b4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67b4f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67b4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67b4f-107">O tipo de política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="67b4f-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="67b4f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="67b4f-108">Members</span></span>
|<span data-ttu-id="67b4f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="67b4f-109">Member</span></span>|<span data-ttu-id="67b4f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="67b4f-110">Value</span></span>|<span data-ttu-id="67b4f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b4f-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="67b4f-112">unknown</span></span>|<span data-ttu-id="67b4f-113">,0</span><span class="sxs-lookup"><span data-stu-id="67b4f-113">0</span></span>|<span data-ttu-id="67b4f-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="67b4f-114">Unknown.</span></span>|
|<span data-ttu-id="67b4f-115">vírus</span><span class="sxs-lookup"><span data-stu-id="67b4f-115">antivirus</span></span>|<span data-ttu-id="67b4f-116">1</span><span class="sxs-lookup"><span data-stu-id="67b4f-116">1</span></span>|<span data-ttu-id="67b4f-117">Vírus.</span><span class="sxs-lookup"><span data-stu-id="67b4f-117">Antivirus.</span></span>|
|<span data-ttu-id="67b4f-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="67b4f-118">diskEncryption</span></span>|<span data-ttu-id="67b4f-119">duas</span><span class="sxs-lookup"><span data-stu-id="67b4f-119">2</span></span>|<span data-ttu-id="67b4f-120">Criptografia de disco.</span><span class="sxs-lookup"><span data-stu-id="67b4f-120">Disk encryption.</span></span>|
|<span data-ttu-id="67b4f-121">Firewall</span><span class="sxs-lookup"><span data-stu-id="67b4f-121">firewall</span></span>|<span data-ttu-id="67b4f-122">3D</span><span class="sxs-lookup"><span data-stu-id="67b4f-122">3</span></span>|<span data-ttu-id="67b4f-123">Firewall.</span><span class="sxs-lookup"><span data-stu-id="67b4f-123">Firewall.</span></span>|
|<span data-ttu-id="67b4f-124">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="67b4f-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="67b4f-125">4 </span><span class="sxs-lookup"><span data-stu-id="67b4f-125">4</span></span>|<span data-ttu-id="67b4f-126">Detecção e resposta do terminal.</span><span class="sxs-lookup"><span data-stu-id="67b4f-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="67b4f-127">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="67b4f-127">attackSurfaceReduction</span></span>|<span data-ttu-id="67b4f-128">5 </span><span class="sxs-lookup"><span data-stu-id="67b4f-128">5</span></span>|<span data-ttu-id="67b4f-129">Redução da superfície do ataque.</span><span class="sxs-lookup"><span data-stu-id="67b4f-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="67b4f-130">accountProtection</span><span class="sxs-lookup"><span data-stu-id="67b4f-130">accountProtection</span></span>|<span data-ttu-id="67b4f-131">6 </span><span class="sxs-lookup"><span data-stu-id="67b4f-131">6</span></span>|<span data-ttu-id="67b4f-132">Proteção de conta.</span><span class="sxs-lookup"><span data-stu-id="67b4f-132">Account protection.</span></span>|



