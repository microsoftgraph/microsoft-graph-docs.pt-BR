---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f76a0b685a0759a4455d8de805424ddd09758a63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970280"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="db499-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="db499-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="db499-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db499-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db499-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db499-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db499-106">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="db499-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="db499-107">Membros</span><span class="sxs-lookup"><span data-stu-id="db499-107">Members</span></span>
|<span data-ttu-id="db499-108">Membro</span><span class="sxs-lookup"><span data-stu-id="db499-108">Member</span></span>|<span data-ttu-id="db499-109">Valor</span><span class="sxs-lookup"><span data-stu-id="db499-109">Value</span></span>|<span data-ttu-id="db499-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db499-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db499-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="db499-111">lmAndNltm</span></span>|<span data-ttu-id="db499-112">,0</span><span class="sxs-lookup"><span data-stu-id="db499-112">0</span></span>|<span data-ttu-id="db499-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="db499-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="db499-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="db499-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="db499-115">1</span><span class="sxs-lookup"><span data-stu-id="db499-115">1</span></span>|<span data-ttu-id="db499-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="db499-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="db499-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="db499-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="db499-118">duas</span><span class="sxs-lookup"><span data-stu-id="db499-118">2</span></span>|<span data-ttu-id="db499-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="db499-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="db499-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="db499-120">lmAndNtlmV2</span></span>|<span data-ttu-id="db499-121">3D</span><span class="sxs-lookup"><span data-stu-id="db499-121">3</span></span>|<span data-ttu-id="db499-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="db499-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="db499-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="db499-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="db499-124">quatro</span><span class="sxs-lookup"><span data-stu-id="db499-124">4</span></span>|<span data-ttu-id="db499-125">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="db499-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="db499-126">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="db499-126">Refuse LM</span></span>|
|<span data-ttu-id="db499-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="db499-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="db499-128">0,5</span><span class="sxs-lookup"><span data-stu-id="db499-128">5</span></span>|<span data-ttu-id="db499-129">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="db499-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="db499-130">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="db499-130">Refuse LM & NTLM</span></span>|





