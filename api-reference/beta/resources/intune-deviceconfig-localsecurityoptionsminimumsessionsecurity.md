---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ab015e80b276870e663d47a3b8b18d17fed82a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946165"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="a3102-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="a3102-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="a3102-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3102-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3102-106">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="a3102-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="a3102-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a3102-107">Members</span></span>
|<span data-ttu-id="a3102-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a3102-108">Member</span></span>|<span data-ttu-id="a3102-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a3102-109">Value</span></span>|<span data-ttu-id="a3102-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3102-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3102-111">none</span><span class="sxs-lookup"><span data-stu-id="a3102-111">none</span></span>|<span data-ttu-id="a3102-112">,0</span><span class="sxs-lookup"><span data-stu-id="a3102-112">0</span></span>|<span data-ttu-id="a3102-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="a3102-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="a3102-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="a3102-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="a3102-115">1</span><span class="sxs-lookup"><span data-stu-id="a3102-115">1</span></span>|<span data-ttu-id="a3102-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="a3102-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="a3102-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="a3102-117">require128BitEncryption</span></span>|<span data-ttu-id="a3102-118">duas</span><span class="sxs-lookup"><span data-stu-id="a3102-118">2</span></span>|<span data-ttu-id="a3102-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="a3102-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="a3102-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="a3102-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="a3102-121">3D</span><span class="sxs-lookup"><span data-stu-id="a3102-121">3</span></span>|<span data-ttu-id="a3102-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="a3102-122">Send LM & NTLMv2 responses only</span></span>|




