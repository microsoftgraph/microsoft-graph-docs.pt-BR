---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7fd08d1ce3dd40e3c60c8cbc42985f4014e1f332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269025"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="12493-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="12493-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="12493-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12493-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12493-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12493-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12493-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12493-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12493-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="12493-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="12493-108">Membros</span><span class="sxs-lookup"><span data-stu-id="12493-108">Members</span></span>
|<span data-ttu-id="12493-109">Membro</span><span class="sxs-lookup"><span data-stu-id="12493-109">Member</span></span>|<span data-ttu-id="12493-110">Valor</span><span class="sxs-lookup"><span data-stu-id="12493-110">Value</span></span>|<span data-ttu-id="12493-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="12493-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12493-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="12493-112">lmAndNltm</span></span>|<span data-ttu-id="12493-113">,0</span><span class="sxs-lookup"><span data-stu-id="12493-113">0</span></span>|<span data-ttu-id="12493-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="12493-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="12493-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="12493-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="12493-116">1</span><span class="sxs-lookup"><span data-stu-id="12493-116">1</span></span>|<span data-ttu-id="12493-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="12493-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="12493-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="12493-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="12493-119">duas</span><span class="sxs-lookup"><span data-stu-id="12493-119">2</span></span>|<span data-ttu-id="12493-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="12493-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="12493-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="12493-121">lmAndNtlmV2</span></span>|<span data-ttu-id="12493-122">3D</span><span class="sxs-lookup"><span data-stu-id="12493-122">3</span></span>|<span data-ttu-id="12493-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="12493-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="12493-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="12493-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="12493-125">4 </span><span class="sxs-lookup"><span data-stu-id="12493-125">4</span></span>|<span data-ttu-id="12493-126">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="12493-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="12493-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="12493-127">Refuse LM</span></span>|
|<span data-ttu-id="12493-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="12493-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="12493-129">5 </span><span class="sxs-lookup"><span data-stu-id="12493-129">5</span></span>|<span data-ttu-id="12493-130">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="12493-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="12493-131">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="12493-131">Refuse LM & NTLM</span></span>|




