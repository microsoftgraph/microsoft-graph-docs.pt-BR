---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397453"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="17809-103">tipo de enum lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="17809-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="17809-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="17809-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17809-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17809-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17809-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="17809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17809-107">Valores possíveis para LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="17809-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="17809-108">Membros</span><span class="sxs-lookup"><span data-stu-id="17809-108">Members</span></span>
|<span data-ttu-id="17809-109">Membro</span><span class="sxs-lookup"><span data-stu-id="17809-109">Member</span></span>|<span data-ttu-id="17809-110">Valor</span><span class="sxs-lookup"><span data-stu-id="17809-110">Value</span></span>|<span data-ttu-id="17809-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17809-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17809-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="17809-112">lmAndNltm</span></span>|<span data-ttu-id="17809-113">0</span><span class="sxs-lookup"><span data-stu-id="17809-113">0</span></span>|<span data-ttu-id="17809-114">Enviar LM & respostas NTLM</span><span class="sxs-lookup"><span data-stu-id="17809-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="17809-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="17809-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="17809-116">1</span><span class="sxs-lookup"><span data-stu-id="17809-116">1</span></span>|<span data-ttu-id="17809-117">Enviar a segurança da sessão do LM & usar NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="17809-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="17809-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="17809-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="17809-119">2</span><span class="sxs-lookup"><span data-stu-id="17809-119">2</span></span>|<span data-ttu-id="17809-120">Enviar LM & somente respostas NTLM</span><span class="sxs-lookup"><span data-stu-id="17809-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="17809-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="17809-121">lmAndNtlmV2</span></span>|<span data-ttu-id="17809-122">3</span><span class="sxs-lookup"><span data-stu-id="17809-122">3</span></span>|<span data-ttu-id="17809-123">Enviar LM & respostas NTLMv2</span><span class="sxs-lookup"><span data-stu-id="17809-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="17809-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="17809-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="17809-125">4</span><span class="sxs-lookup"><span data-stu-id="17809-125">4</span></span>|<span data-ttu-id="17809-126">Envie LM & respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="17809-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="17809-127">Recusar LM</span><span class="sxs-lookup"><span data-stu-id="17809-127">Refuse LM</span></span>|
|<span data-ttu-id="17809-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="17809-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="17809-129">5</span><span class="sxs-lookup"><span data-stu-id="17809-129">5</span></span>|<span data-ttu-id="17809-130">Envie LM & respostas NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="17809-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="17809-131">Recusar LM e NTLM &</span><span class="sxs-lookup"><span data-stu-id="17809-131">Refuse LM & NTLM</span></span>|




