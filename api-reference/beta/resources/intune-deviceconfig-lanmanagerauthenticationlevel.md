---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866910"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="186ab-103">tipo de enum lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="186ab-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="186ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="186ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="186ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="186ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="186ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="186ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="186ab-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="186ab-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="186ab-108">Membros</span><span class="sxs-lookup"><span data-stu-id="186ab-108">Members</span></span>
|<span data-ttu-id="186ab-109">Membro</span><span class="sxs-lookup"><span data-stu-id="186ab-109">Member</span></span>|<span data-ttu-id="186ab-110">Valor</span><span class="sxs-lookup"><span data-stu-id="186ab-110">Value</span></span>|<span data-ttu-id="186ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="186ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186ab-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="186ab-112">lmAndNltm</span></span>|<span data-ttu-id="186ab-113">0</span><span class="sxs-lookup"><span data-stu-id="186ab-113">0</span></span>|<span data-ttu-id="186ab-114">Enviar respostas LM e NTLM</span><span class="sxs-lookup"><span data-stu-id="186ab-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="186ab-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="186ab-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="186ab-116">1</span><span class="sxs-lookup"><span data-stu-id="186ab-116">1</span></span>|<span data-ttu-id="186ab-117">Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="186ab-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="186ab-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="186ab-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="186ab-119">2</span><span class="sxs-lookup"><span data-stu-id="186ab-119">2</span></span>|<span data-ttu-id="186ab-120">Enviar respostas LM & NTLM somente</span><span class="sxs-lookup"><span data-stu-id="186ab-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="186ab-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="186ab-121">lmAndNtlmV2</span></span>|<span data-ttu-id="186ab-122">3</span><span class="sxs-lookup"><span data-stu-id="186ab-122">3</span></span>|<span data-ttu-id="186ab-123">Enviar respostas LM & NTLMv2 somente</span><span class="sxs-lookup"><span data-stu-id="186ab-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="186ab-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="186ab-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="186ab-125">4</span><span class="sxs-lookup"><span data-stu-id="186ab-125">4</span></span>|<span data-ttu-id="186ab-126">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="186ab-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="186ab-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="186ab-127">Refuse LM</span></span>|
|<span data-ttu-id="186ab-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="186ab-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="186ab-129">5</span><span class="sxs-lookup"><span data-stu-id="186ab-129">5</span></span>|<span data-ttu-id="186ab-130">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="186ab-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="186ab-131">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="186ab-131">Refuse LM & NTLM</span></span>|





