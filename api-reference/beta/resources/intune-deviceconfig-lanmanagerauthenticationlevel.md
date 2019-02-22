---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166567"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="c7535-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="c7535-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="c7535-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7535-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7535-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7535-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7535-106">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="c7535-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="c7535-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c7535-107">Members</span></span>
|<span data-ttu-id="c7535-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c7535-108">Member</span></span>|<span data-ttu-id="c7535-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c7535-109">Value</span></span>|<span data-ttu-id="c7535-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7535-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7535-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="c7535-111">lmAndNltm</span></span>|<span data-ttu-id="c7535-112">,0</span><span class="sxs-lookup"><span data-stu-id="c7535-112">0</span></span>|<span data-ttu-id="c7535-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c7535-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="c7535-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c7535-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="c7535-115">1</span><span class="sxs-lookup"><span data-stu-id="c7535-115">1</span></span>|<span data-ttu-id="c7535-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="c7535-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="c7535-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="c7535-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="c7535-118">duas</span><span class="sxs-lookup"><span data-stu-id="c7535-118">2</span></span>|<span data-ttu-id="c7535-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c7535-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="c7535-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c7535-120">lmAndNtlmV2</span></span>|<span data-ttu-id="c7535-121">3D</span><span class="sxs-lookup"><span data-stu-id="c7535-121">3</span></span>|<span data-ttu-id="c7535-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="c7535-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="c7535-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="c7535-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="c7535-124">quatro</span><span class="sxs-lookup"><span data-stu-id="c7535-124">4</span></span>|<span data-ttu-id="c7535-125">Enviar somente respostas LM & NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="c7535-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c7535-126">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="c7535-126">Refuse LM</span></span>|
|<span data-ttu-id="c7535-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="c7535-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="c7535-128">0,5</span><span class="sxs-lookup"><span data-stu-id="c7535-128">5</span></span>|<span data-ttu-id="c7535-129">Enviar somente respostas LM & NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="c7535-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c7535-130">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c7535-130">Refuse LM & NTLM</span></span>|




