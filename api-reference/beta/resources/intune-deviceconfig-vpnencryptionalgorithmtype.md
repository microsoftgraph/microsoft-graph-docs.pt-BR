---
title: tipo de enumeração vpnEncryptionAlgorithmType
description: O tipo de algoritmo de criptografia de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b8a14effae7c95605529c0d0b12eb45f51708c43
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788154"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="9e618-103">tipo de enumeração vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="9e618-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="9e618-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e618-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e618-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e618-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e618-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e618-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e618-107">O tipo de algoritmo de criptografia de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="9e618-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="9e618-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9e618-108">Members</span></span>
|<span data-ttu-id="9e618-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9e618-109">Member</span></span>|<span data-ttu-id="9e618-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9e618-110">Value</span></span>|<span data-ttu-id="9e618-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e618-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e618-112">aes256</span><span class="sxs-lookup"><span data-stu-id="9e618-112">aes256</span></span>|<span data-ttu-id="9e618-113">,0</span><span class="sxs-lookup"><span data-stu-id="9e618-113">0</span></span>|<span data-ttu-id="9e618-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="9e618-114">AES-256</span></span>|
|<span data-ttu-id="9e618-115">criptografia</span><span class="sxs-lookup"><span data-stu-id="9e618-115">des</span></span>|<span data-ttu-id="9e618-116">1 </span><span class="sxs-lookup"><span data-stu-id="9e618-116">1</span></span>|<span data-ttu-id="9e618-117">CRIPTOGRAFIA</span><span class="sxs-lookup"><span data-stu-id="9e618-117">DES</span></span>|
|<span data-ttu-id="9e618-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="9e618-118">tripleDes</span></span>|<span data-ttu-id="9e618-119">duas</span><span class="sxs-lookup"><span data-stu-id="9e618-119">2</span></span>|<span data-ttu-id="9e618-120">ALGORITMO</span><span class="sxs-lookup"><span data-stu-id="9e618-120">3DES</span></span>|
|<span data-ttu-id="9e618-121">aes128</span><span class="sxs-lookup"><span data-stu-id="9e618-121">aes128</span></span>|<span data-ttu-id="9e618-122">3D</span><span class="sxs-lookup"><span data-stu-id="9e618-122">3</span></span>|<span data-ttu-id="9e618-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="9e618-123">AES-128</span></span>|
|<span data-ttu-id="9e618-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="9e618-124">aes128Gcm</span></span>|<span data-ttu-id="9e618-125">4 </span><span class="sxs-lookup"><span data-stu-id="9e618-125">4</span></span>|<span data-ttu-id="9e618-126">AES-128-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="9e618-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="9e618-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="9e618-127">aes256Gcm</span></span>|<span data-ttu-id="9e618-128">5 </span><span class="sxs-lookup"><span data-stu-id="9e618-128">5</span></span>|<span data-ttu-id="9e618-129">AES-256-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="9e618-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="9e618-130">aes192</span><span class="sxs-lookup"><span data-stu-id="9e618-130">aes192</span></span>|<span data-ttu-id="9e618-131">6 </span><span class="sxs-lookup"><span data-stu-id="9e618-131">6</span></span>|<span data-ttu-id="9e618-132">AES-192</span><span class="sxs-lookup"><span data-stu-id="9e618-132">AES-192</span></span>|
|<span data-ttu-id="9e618-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="9e618-133">aes192Gcm</span></span>|<span data-ttu-id="9e618-134">7 </span><span class="sxs-lookup"><span data-stu-id="9e618-134">7</span></span>|<span data-ttu-id="9e618-135">AES-192-GCM</span><span class="sxs-lookup"><span data-stu-id="9e618-135">AES-192-GCM</span></span>|



