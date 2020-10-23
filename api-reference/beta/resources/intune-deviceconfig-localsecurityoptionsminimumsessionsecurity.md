---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 408e94fa12e0776d4d36fb85319ea16d4bf514e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726448"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="8b6f5-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8b6f5-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="8b6f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b6f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b6f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b6f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b6f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b6f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b6f5-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8b6f5-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="8b6f5-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8b6f5-108">Members</span></span>
|<span data-ttu-id="8b6f5-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8b6f5-109">Member</span></span>|<span data-ttu-id="8b6f5-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8b6f5-110">Value</span></span>|<span data-ttu-id="8b6f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b6f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b6f5-112">none</span><span class="sxs-lookup"><span data-stu-id="8b6f5-112">none</span></span>|<span data-ttu-id="8b6f5-113">,0</span><span class="sxs-lookup"><span data-stu-id="8b6f5-113">0</span></span>|<span data-ttu-id="8b6f5-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="8b6f5-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="8b6f5-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8b6f5-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="8b6f5-116">1</span><span class="sxs-lookup"><span data-stu-id="8b6f5-116">1</span></span>|<span data-ttu-id="8b6f5-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="8b6f5-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="8b6f5-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8b6f5-118">require128BitEncryption</span></span>|<span data-ttu-id="8b6f5-119">duas</span><span class="sxs-lookup"><span data-stu-id="8b6f5-119">2</span></span>|<span data-ttu-id="8b6f5-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="8b6f5-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="8b6f5-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8b6f5-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="8b6f5-122">3D</span><span class="sxs-lookup"><span data-stu-id="8b6f5-122">3</span></span>|<span data-ttu-id="8b6f5-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="8b6f5-123">Send LM & NTLMv2 responses only</span></span>|





