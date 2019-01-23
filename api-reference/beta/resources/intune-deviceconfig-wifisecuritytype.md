---
title: tipo de enum wiFiSecurityType
description: Tipos de segurança Wi-Fi.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422128"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="a5b8e-103">tipo de enum wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a5b8e-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="a5b8e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5b8e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5b8e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5b8e-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="a5b8e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a5b8e-108">Members</span></span>
|<span data-ttu-id="a5b8e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a5b8e-109">Member</span></span>|<span data-ttu-id="a5b8e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a5b8e-110">Value</span></span>|<span data-ttu-id="a5b8e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b8e-112">Abrir</span><span class="sxs-lookup"><span data-stu-id="a5b8e-112">open</span></span>|<span data-ttu-id="a5b8e-113">0</span><span class="sxs-lookup"><span data-stu-id="a5b8e-113">0</span></span>|<span data-ttu-id="a5b8e-114">Abra (nenhuma autenticação).</span><span class="sxs-lookup"><span data-stu-id="a5b8e-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="a5b8e-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="a5b8e-115">wpaPersonal</span></span>|<span data-ttu-id="a5b8e-116">1</span><span class="sxs-lookup"><span data-stu-id="a5b8e-116">1</span></span>|<span data-ttu-id="a5b8e-117">WPA-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-117">WPA-Personal.</span></span>|
|<span data-ttu-id="a5b8e-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="a5b8e-118">wpaEnterprise</span></span>|<span data-ttu-id="a5b8e-119">2</span><span class="sxs-lookup"><span data-stu-id="a5b8e-119">2</span></span>|<span data-ttu-id="a5b8e-120">WPA-Empresa.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-120">WPA-Enterprise.</span></span> <span data-ttu-id="a5b8e-121">Deve usar o tipo de IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="a5b8e-122">WEP</span><span class="sxs-lookup"><span data-stu-id="a5b8e-122">wep</span></span>|<span data-ttu-id="a5b8e-123">3</span><span class="sxs-lookup"><span data-stu-id="a5b8e-123">3</span></span>|<span data-ttu-id="a5b8e-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-124">WEP Encryption.</span></span>|
|<span data-ttu-id="a5b8e-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="a5b8e-125">wpa2Personal</span></span>|<span data-ttu-id="a5b8e-126">4</span><span class="sxs-lookup"><span data-stu-id="a5b8e-126">4</span></span>|<span data-ttu-id="a5b8e-127">WPA2-pessoal.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="a5b8e-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="a5b8e-128">wpa2Enterprise</span></span>|<span data-ttu-id="a5b8e-129">5</span><span class="sxs-lookup"><span data-stu-id="a5b8e-129">5</span></span>|<span data-ttu-id="a5b8e-130">WPA2-Empresa.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-130">WPA2-Enterprise.</span></span> <span data-ttu-id="a5b8e-131">Deve usar o tipo de WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="a5b8e-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




