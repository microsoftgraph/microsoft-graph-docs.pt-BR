---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a80aefec83c0c2a577af9b8dfed5dcea1ff7d79
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989347"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="4c317-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4c317-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="4c317-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c317-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c317-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c317-106">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4c317-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="4c317-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4c317-107">Members</span></span>
|<span data-ttu-id="4c317-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4c317-108">Member</span></span>|<span data-ttu-id="4c317-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4c317-109">Value</span></span>|<span data-ttu-id="4c317-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c317-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c317-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="4c317-111">lmAndNltm</span></span>|<span data-ttu-id="4c317-112">,0</span><span class="sxs-lookup"><span data-stu-id="4c317-112">0</span></span>|<span data-ttu-id="4c317-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4c317-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="4c317-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4c317-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="4c317-115">1</span><span class="sxs-lookup"><span data-stu-id="4c317-115">1</span></span>|<span data-ttu-id="4c317-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="4c317-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="4c317-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="4c317-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="4c317-118">duas</span><span class="sxs-lookup"><span data-stu-id="4c317-118">2</span></span>|<span data-ttu-id="4c317-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4c317-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="4c317-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4c317-120">lmAndNtlmV2</span></span>|<span data-ttu-id="4c317-121">3D</span><span class="sxs-lookup"><span data-stu-id="4c317-121">3</span></span>|<span data-ttu-id="4c317-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="4c317-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="4c317-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="4c317-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="4c317-124">quatro</span><span class="sxs-lookup"><span data-stu-id="4c317-124">4</span></span>|<span data-ttu-id="4c317-125">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="4c317-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4c317-126">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="4c317-126">Refuse LM</span></span>|
|<span data-ttu-id="4c317-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="4c317-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="4c317-128">0,5</span><span class="sxs-lookup"><span data-stu-id="4c317-128">5</span></span>|<span data-ttu-id="4c317-129">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="4c317-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4c317-130">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4c317-130">Refuse LM & NTLM</span></span>|





