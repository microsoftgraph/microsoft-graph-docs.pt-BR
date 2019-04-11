---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801243"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="1f303-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1f303-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="1f303-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f303-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f303-106">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1f303-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="1f303-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1f303-107">Members</span></span>
|<span data-ttu-id="1f303-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1f303-108">Member</span></span>|<span data-ttu-id="1f303-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1f303-109">Value</span></span>|<span data-ttu-id="1f303-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f303-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f303-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="1f303-111">lmAndNltm</span></span>|<span data-ttu-id="1f303-112">,0</span><span class="sxs-lookup"><span data-stu-id="1f303-112">0</span></span>|<span data-ttu-id="1f303-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1f303-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="1f303-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="1f303-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="1f303-115">1</span><span class="sxs-lookup"><span data-stu-id="1f303-115">1</span></span>|<span data-ttu-id="1f303-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="1f303-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="1f303-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="1f303-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="1f303-118">duas</span><span class="sxs-lookup"><span data-stu-id="1f303-118">2</span></span>|<span data-ttu-id="1f303-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1f303-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="1f303-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="1f303-120">lmAndNtlmV2</span></span>|<span data-ttu-id="1f303-121">3D</span><span class="sxs-lookup"><span data-stu-id="1f303-121">3</span></span>|<span data-ttu-id="1f303-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="1f303-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="1f303-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="1f303-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="1f303-124">quatro</span><span class="sxs-lookup"><span data-stu-id="1f303-124">4</span></span>|<span data-ttu-id="1f303-125">Enviar somente respostas LM & NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="1f303-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="1f303-126">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="1f303-126">Refuse LM</span></span>|
|<span data-ttu-id="1f303-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="1f303-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="1f303-128">0,5</span><span class="sxs-lookup"><span data-stu-id="1f303-128">5</span></span>|<span data-ttu-id="1f303-129">Enviar somente respostas LM & NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="1f303-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="1f303-130">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1f303-130">Refuse LM & NTLM</span></span>|





