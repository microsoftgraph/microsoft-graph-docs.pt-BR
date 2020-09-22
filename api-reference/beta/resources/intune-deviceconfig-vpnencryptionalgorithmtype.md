---
title: tipo de enumeração vpnEncryptionAlgorithmType
description: O tipo de algoritmo de criptografia de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c8a07e6e1eb5190457b5c66630a9595264334cd1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049106"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="6d99b-103">tipo de enumeração vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="6d99b-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="6d99b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d99b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d99b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d99b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d99b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d99b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d99b-107">O tipo de algoritmo de criptografia de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="6d99b-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="6d99b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6d99b-108">Members</span></span>
|<span data-ttu-id="6d99b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6d99b-109">Member</span></span>|<span data-ttu-id="6d99b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6d99b-110">Value</span></span>|<span data-ttu-id="6d99b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d99b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d99b-112">aes256</span><span class="sxs-lookup"><span data-stu-id="6d99b-112">aes256</span></span>|<span data-ttu-id="6d99b-113">,0</span><span class="sxs-lookup"><span data-stu-id="6d99b-113">0</span></span>|<span data-ttu-id="6d99b-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="6d99b-114">AES-256</span></span>|
|<span data-ttu-id="6d99b-115">criptografia</span><span class="sxs-lookup"><span data-stu-id="6d99b-115">des</span></span>|<span data-ttu-id="6d99b-116">1 </span><span class="sxs-lookup"><span data-stu-id="6d99b-116">1</span></span>|<span data-ttu-id="6d99b-117">CRIPTOGRAFIA</span><span class="sxs-lookup"><span data-stu-id="6d99b-117">DES</span></span>|
|<span data-ttu-id="6d99b-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="6d99b-118">tripleDes</span></span>|<span data-ttu-id="6d99b-119">2 </span><span class="sxs-lookup"><span data-stu-id="6d99b-119">2</span></span>|<span data-ttu-id="6d99b-120">ALGORITMO</span><span class="sxs-lookup"><span data-stu-id="6d99b-120">3DES</span></span>|
|<span data-ttu-id="6d99b-121">aes128</span><span class="sxs-lookup"><span data-stu-id="6d99b-121">aes128</span></span>|<span data-ttu-id="6d99b-122">3 </span><span class="sxs-lookup"><span data-stu-id="6d99b-122">3</span></span>|<span data-ttu-id="6d99b-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="6d99b-123">AES-128</span></span>|
|<span data-ttu-id="6d99b-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="6d99b-124">aes128Gcm</span></span>|<span data-ttu-id="6d99b-125">4 </span><span class="sxs-lookup"><span data-stu-id="6d99b-125">4</span></span>|<span data-ttu-id="6d99b-126">AES-128-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="6d99b-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="6d99b-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="6d99b-127">aes256Gcm</span></span>|<span data-ttu-id="6d99b-128">5 </span><span class="sxs-lookup"><span data-stu-id="6d99b-128">5</span></span>|<span data-ttu-id="6d99b-129">AES-256-GCM (16 octeto do ICV)</span><span class="sxs-lookup"><span data-stu-id="6d99b-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="6d99b-130">aes192</span><span class="sxs-lookup"><span data-stu-id="6d99b-130">aes192</span></span>|<span data-ttu-id="6d99b-131">6 </span><span class="sxs-lookup"><span data-stu-id="6d99b-131">6</span></span>|<span data-ttu-id="6d99b-132">AES-192</span><span class="sxs-lookup"><span data-stu-id="6d99b-132">AES-192</span></span>|
|<span data-ttu-id="6d99b-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="6d99b-133">aes192Gcm</span></span>|<span data-ttu-id="6d99b-134">7 </span><span class="sxs-lookup"><span data-stu-id="6d99b-134">7</span></span>|<span data-ttu-id="6d99b-135">AES-192-GCM</span><span class="sxs-lookup"><span data-stu-id="6d99b-135">AES-192-GCM</span></span>|






