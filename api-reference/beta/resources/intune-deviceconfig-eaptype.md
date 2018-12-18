---
title: tipo de enum eapType
description: Tipos de configuração de autenticação EAP (Protocol) extensível.
author: tfitzmac
ms.openlocfilehash: e95924209b8137a1c5d35896c0195e9e962d7af9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319541"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="c0d0c-103">tipo de enum eapType</span><span class="sxs-lookup"><span data-stu-id="c0d0c-103">eapType enum type</span></span>

> <span data-ttu-id="c0d0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0d0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0d0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0d0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0d0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0d0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0d0c-107">Tipos de configuração de autenticação EAP (Protocol) extensível.</span><span class="sxs-lookup"><span data-stu-id="c0d0c-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="c0d0c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c0d0c-108">Members</span></span>
|<span data-ttu-id="c0d0c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c0d0c-109">Member</span></span>|<span data-ttu-id="c0d0c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c0d0c-110">Value</span></span>|<span data-ttu-id="c0d0c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0d0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0d0c-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="c0d0c-112">eapTls</span></span>|<span data-ttu-id="c0d0c-113">13</span><span class="sxs-lookup"><span data-stu-id="c0d0c-113">13</span></span>|<span data-ttu-id="c0d0c-114">EAP-Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="c0d0c-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="c0d0c-115">salto</span><span class="sxs-lookup"><span data-stu-id="c0d0c-115">leap</span></span>|<span data-ttu-id="c0d0c-116">17</span><span class="sxs-lookup"><span data-stu-id="c0d0c-116">17</span></span>|<span data-ttu-id="c0d0c-117">Protocolo de autenticação extensível leve (SALTO).</span><span class="sxs-lookup"><span data-stu-id="c0d0c-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="c0d0c-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="c0d0c-118">eapSim</span></span>|<span data-ttu-id="c0d0c-119">18</span><span class="sxs-lookup"><span data-stu-id="c0d0c-119">18</span></span>|<span data-ttu-id="c0d0c-120">EAP para o módulo de identidade do assinante GSM (EAP-SIM).</span><span class="sxs-lookup"><span data-stu-id="c0d0c-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="c0d0c-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="c0d0c-121">eapTtls</span></span>|<span data-ttu-id="c0d0c-122">21</span><span class="sxs-lookup"><span data-stu-id="c0d0c-122">21</span></span>|<span data-ttu-id="c0d0c-123">EAP-encapsulada Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="c0d0c-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="c0d0c-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="c0d0c-124">peap</span></span>|<span data-ttu-id="c0d0c-125">25</span><span class="sxs-lookup"><span data-stu-id="c0d0c-125">25</span></span>|<span data-ttu-id="c0d0c-126">Protegido (PEAP) do protocolo de autenticação extensível.</span><span class="sxs-lookup"><span data-stu-id="c0d0c-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="c0d0c-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="c0d0c-127">eapFast</span></span>|<span data-ttu-id="c0d0c-128">43</span><span class="sxs-lookup"><span data-stu-id="c0d0c-128">43</span></span>|<span data-ttu-id="c0d0c-129">Autenticação EAP flexíveis via seguro encapsulamento (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="c0d0c-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





