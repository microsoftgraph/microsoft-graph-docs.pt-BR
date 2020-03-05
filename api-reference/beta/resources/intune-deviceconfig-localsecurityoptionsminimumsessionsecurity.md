---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4750d5bc4da34f1e627d2b324827f78f830bb219
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526217"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="1200d-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1200d-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="1200d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1200d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1200d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1200d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1200d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1200d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1200d-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1200d-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="1200d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1200d-108">Members</span></span>
|<span data-ttu-id="1200d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1200d-109">Member</span></span>|<span data-ttu-id="1200d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1200d-110">Value</span></span>|<span data-ttu-id="1200d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1200d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1200d-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="1200d-112">none</span></span>|<span data-ttu-id="1200d-113">,0</span><span class="sxs-lookup"><span data-stu-id="1200d-113">0</span></span>|<span data-ttu-id="1200d-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1200d-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="1200d-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1200d-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="1200d-116">1 </span><span class="sxs-lookup"><span data-stu-id="1200d-116">1</span></span>|<span data-ttu-id="1200d-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="1200d-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="1200d-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="1200d-118">require128BitEncryption</span></span>|<span data-ttu-id="1200d-119">2 </span><span class="sxs-lookup"><span data-stu-id="1200d-119">2</span></span>|<span data-ttu-id="1200d-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1200d-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="1200d-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="1200d-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="1200d-122">3 </span><span class="sxs-lookup"><span data-stu-id="1200d-122">3</span></span>|<span data-ttu-id="1200d-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="1200d-123">Send LM & NTLMv2 responses only</span></span>|



