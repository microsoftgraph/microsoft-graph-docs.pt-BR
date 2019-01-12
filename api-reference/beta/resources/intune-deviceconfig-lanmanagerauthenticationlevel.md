---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911991"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="ced8f-103">tipo de enum lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="ced8f-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="ced8f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ced8f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ced8f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ced8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ced8f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ced8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ced8f-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="ced8f-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="ced8f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ced8f-108">Members</span></span>
|<span data-ttu-id="ced8f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ced8f-109">Member</span></span>|<span data-ttu-id="ced8f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ced8f-110">Value</span></span>|<span data-ttu-id="ced8f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ced8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced8f-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="ced8f-112">lmAndNltm</span></span>|<span data-ttu-id="ced8f-113">0</span><span class="sxs-lookup"><span data-stu-id="ced8f-113">0</span></span>|<span data-ttu-id="ced8f-114">Enviar respostas LM e NTLM</span><span class="sxs-lookup"><span data-stu-id="ced8f-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="ced8f-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="ced8f-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="ced8f-116">1</span><span class="sxs-lookup"><span data-stu-id="ced8f-116">1</span></span>|<span data-ttu-id="ced8f-117">Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="ced8f-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="ced8f-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="ced8f-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="ced8f-119">2</span><span class="sxs-lookup"><span data-stu-id="ced8f-119">2</span></span>|<span data-ttu-id="ced8f-120">Enviar respostas LM & NTLM somente</span><span class="sxs-lookup"><span data-stu-id="ced8f-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="ced8f-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="ced8f-121">lmAndNtlmV2</span></span>|<span data-ttu-id="ced8f-122">3</span><span class="sxs-lookup"><span data-stu-id="ced8f-122">3</span></span>|<span data-ttu-id="ced8f-123">Enviar respostas LM & NTLMv2 somente</span><span class="sxs-lookup"><span data-stu-id="ced8f-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="ced8f-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="ced8f-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="ced8f-125">4</span><span class="sxs-lookup"><span data-stu-id="ced8f-125">4</span></span>|<span data-ttu-id="ced8f-126">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="ced8f-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="ced8f-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="ced8f-127">Refuse LM</span></span>|
|<span data-ttu-id="ced8f-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="ced8f-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="ced8f-129">5</span><span class="sxs-lookup"><span data-stu-id="ced8f-129">5</span></span>|<span data-ttu-id="ced8f-130">Envie respostas LM & NTLMv2 apenas.</span><span class="sxs-lookup"><span data-stu-id="ced8f-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="ced8f-131">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="ced8f-131">Refuse LM & NTLM</span></span>|





