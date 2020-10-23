---
title: tipo de enumeração vpnEncryptionAlgorithmType
description: O tipo de algoritmo de criptografia de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 420dff0b05cae2bb403b7f8746063fc3417c4a4f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728367"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="ea368-103">tipo de enumeração vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="ea368-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="ea368-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea368-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea368-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea368-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea368-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea368-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea368-107">O tipo de algoritmo de criptografia de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="ea368-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="ea368-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ea368-108">Members</span></span>
|<span data-ttu-id="ea368-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ea368-109">Member</span></span>|<span data-ttu-id="ea368-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ea368-110">Value</span></span>|<span data-ttu-id="ea368-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea368-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea368-112">aes256</span><span class="sxs-lookup"><span data-stu-id="ea368-112">aes256</span></span>|<span data-ttu-id="ea368-113">,0</span><span class="sxs-lookup"><span data-stu-id="ea368-113">0</span></span>|<span data-ttu-id="ea368-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="ea368-114">AES-256</span></span>|
|<span data-ttu-id="ea368-115">criptografia</span><span class="sxs-lookup"><span data-stu-id="ea368-115">des</span></span>|<span data-ttu-id="ea368-116">1</span><span class="sxs-lookup"><span data-stu-id="ea368-116">1</span></span>|<span data-ttu-id="ea368-117">CRIPTOGRAFIA</span><span class="sxs-lookup"><span data-stu-id="ea368-117">DES</span></span>|
|<span data-ttu-id="ea368-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="ea368-118">tripleDes</span></span>|<span data-ttu-id="ea368-119">duas</span><span class="sxs-lookup"><span data-stu-id="ea368-119">2</span></span>|<span data-ttu-id="ea368-120">ALGORITMO</span><span class="sxs-lookup"><span data-stu-id="ea368-120">3DES</span></span>|
|<span data-ttu-id="ea368-121">aes128</span><span class="sxs-lookup"><span data-stu-id="ea368-121">aes128</span></span>|<span data-ttu-id="ea368-122">3D</span><span class="sxs-lookup"><span data-stu-id="ea368-122">3</span></span>|<span data-ttu-id="ea368-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="ea368-123">AES-128</span></span>|
|<span data-ttu-id="ea368-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="ea368-124">aes128Gcm</span></span>|<span data-ttu-id="ea368-125">4 </span><span class="sxs-lookup"><span data-stu-id="ea368-125">4</span></span>|<span data-ttu-id="ea368-126">AES-128-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="ea368-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="ea368-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="ea368-127">aes256Gcm</span></span>|<span data-ttu-id="ea368-128">5 </span><span class="sxs-lookup"><span data-stu-id="ea368-128">5</span></span>|<span data-ttu-id="ea368-129">AES-256-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="ea368-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="ea368-130">aes192</span><span class="sxs-lookup"><span data-stu-id="ea368-130">aes192</span></span>|<span data-ttu-id="ea368-131">6 </span><span class="sxs-lookup"><span data-stu-id="ea368-131">6</span></span>|<span data-ttu-id="ea368-132">AES-192</span><span class="sxs-lookup"><span data-stu-id="ea368-132">AES-192</span></span>|
|<span data-ttu-id="ea368-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="ea368-133">aes192Gcm</span></span>|<span data-ttu-id="ea368-134">7 </span><span class="sxs-lookup"><span data-stu-id="ea368-134">7</span></span>|<span data-ttu-id="ea368-135">AES-192-GCM</span><span class="sxs-lookup"><span data-stu-id="ea368-135">AES-192-GCM</span></span>|





