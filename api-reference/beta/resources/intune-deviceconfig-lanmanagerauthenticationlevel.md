---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b979c66469ac29339045dd9d1341f85839084bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529757"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="97fd8-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="97fd8-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="97fd8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="97fd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97fd8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97fd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97fd8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97fd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97fd8-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="97fd8-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="97fd8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="97fd8-108">Members</span></span>
|<span data-ttu-id="97fd8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="97fd8-109">Member</span></span>|<span data-ttu-id="97fd8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="97fd8-110">Value</span></span>|<span data-ttu-id="97fd8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97fd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97fd8-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="97fd8-112">lmAndNltm</span></span>|<span data-ttu-id="97fd8-113">,0</span><span class="sxs-lookup"><span data-stu-id="97fd8-113">0</span></span>|<span data-ttu-id="97fd8-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="97fd8-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="97fd8-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="97fd8-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="97fd8-116">1 </span><span class="sxs-lookup"><span data-stu-id="97fd8-116">1</span></span>|<span data-ttu-id="97fd8-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="97fd8-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="97fd8-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="97fd8-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="97fd8-119">2 </span><span class="sxs-lookup"><span data-stu-id="97fd8-119">2</span></span>|<span data-ttu-id="97fd8-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="97fd8-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="97fd8-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="97fd8-121">lmAndNtlmV2</span></span>|<span data-ttu-id="97fd8-122">3 </span><span class="sxs-lookup"><span data-stu-id="97fd8-122">3</span></span>|<span data-ttu-id="97fd8-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="97fd8-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="97fd8-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="97fd8-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="97fd8-125">4 </span><span class="sxs-lookup"><span data-stu-id="97fd8-125">4</span></span>|<span data-ttu-id="97fd8-126">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="97fd8-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="97fd8-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="97fd8-127">Refuse LM</span></span>|
|<span data-ttu-id="97fd8-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="97fd8-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="97fd8-129">5 </span><span class="sxs-lookup"><span data-stu-id="97fd8-129">5</span></span>|<span data-ttu-id="97fd8-130">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="97fd8-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="97fd8-131">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="97fd8-131">Refuse LM & NTLM</span></span>|



