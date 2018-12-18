---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
ms.openlocfilehash: fd5d63f262b9b6e9a27060725e721cb81c495a57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308740"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="bb3eb-103">tipo de enum lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="bb3eb-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="bb3eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb3eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb3eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb3eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb3eb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb3eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb3eb-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="bb3eb-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="bb3eb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bb3eb-108">Members</span></span>
|<span data-ttu-id="bb3eb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bb3eb-109">Member</span></span>|<span data-ttu-id="bb3eb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bb3eb-110">Value</span></span>|<span data-ttu-id="bb3eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb3eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb3eb-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="bb3eb-112">lmAndNltm</span></span>|<span data-ttu-id="bb3eb-113">0</span><span class="sxs-lookup"><span data-stu-id="bb3eb-113">0</span></span>|<span data-ttu-id="bb3eb-114">Enviar respostas LM e NTLM</span><span class="sxs-lookup"><span data-stu-id="bb3eb-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="bb3eb-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="bb3eb-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="bb3eb-116">1</span><span class="sxs-lookup"><span data-stu-id="bb3eb-116">1</span></span>|<span data-ttu-id="bb3eb-117">Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="bb3eb-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="bb3eb-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="bb3eb-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="bb3eb-119">2</span><span class="sxs-lookup"><span data-stu-id="bb3eb-119">2</span></span>|<span data-ttu-id="bb3eb-120">Enviar respostas LM & NTLM somente</span><span class="sxs-lookup"><span data-stu-id="bb3eb-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="bb3eb-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="bb3eb-121">lmAndNtlmV2</span></span>|<span data-ttu-id="bb3eb-122">3</span><span class="sxs-lookup"><span data-stu-id="bb3eb-122">3</span></span>|<span data-ttu-id="bb3eb-123">Enviar respostas LM & NTLMv2 somente</span><span class="sxs-lookup"><span data-stu-id="bb3eb-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="bb3eb-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="bb3eb-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="bb3eb-125">4</span><span class="sxs-lookup"><span data-stu-id="bb3eb-125">4</span></span>|<span data-ttu-id="bb3eb-126">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="bb3eb-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="bb3eb-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="bb3eb-127">Refuse LM</span></span>|
|<span data-ttu-id="bb3eb-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="bb3eb-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="bb3eb-129">5</span><span class="sxs-lookup"><span data-stu-id="bb3eb-129">5</span></span>|<span data-ttu-id="bb3eb-130">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="bb3eb-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="bb3eb-131">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="bb3eb-131">Refuse LM & NTLM</span></span>|





