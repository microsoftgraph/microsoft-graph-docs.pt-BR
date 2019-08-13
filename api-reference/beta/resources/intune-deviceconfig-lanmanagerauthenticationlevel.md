---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356722"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="07fd2-103">tipo de enumeração lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="07fd2-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="07fd2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07fd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07fd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07fd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07fd2-106">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="07fd2-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="07fd2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="07fd2-107">Members</span></span>
|<span data-ttu-id="07fd2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="07fd2-108">Member</span></span>|<span data-ttu-id="07fd2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="07fd2-109">Value</span></span>|<span data-ttu-id="07fd2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07fd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07fd2-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="07fd2-111">lmAndNltm</span></span>|<span data-ttu-id="07fd2-112">,0</span><span class="sxs-lookup"><span data-stu-id="07fd2-112">0</span></span>|<span data-ttu-id="07fd2-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="07fd2-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="07fd2-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="07fd2-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="07fd2-115">1</span><span class="sxs-lookup"><span data-stu-id="07fd2-115">1</span></span>|<span data-ttu-id="07fd2-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="07fd2-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="07fd2-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="07fd2-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="07fd2-118">duas</span><span class="sxs-lookup"><span data-stu-id="07fd2-118">2</span></span>|<span data-ttu-id="07fd2-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="07fd2-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="07fd2-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="07fd2-120">lmAndNtlmV2</span></span>|<span data-ttu-id="07fd2-121">3D</span><span class="sxs-lookup"><span data-stu-id="07fd2-121">3</span></span>|<span data-ttu-id="07fd2-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="07fd2-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="07fd2-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="07fd2-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="07fd2-124">quatro</span><span class="sxs-lookup"><span data-stu-id="07fd2-124">4</span></span>|<span data-ttu-id="07fd2-125">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="07fd2-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="07fd2-126">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="07fd2-126">Refuse LM</span></span>|
|<span data-ttu-id="07fd2-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="07fd2-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="07fd2-128">0,5</span><span class="sxs-lookup"><span data-stu-id="07fd2-128">5</span></span>|<span data-ttu-id="07fd2-129">Enviar LM & somente respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="07fd2-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="07fd2-130">Recusar LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="07fd2-130">Refuse LM & NTLM</span></span>|



