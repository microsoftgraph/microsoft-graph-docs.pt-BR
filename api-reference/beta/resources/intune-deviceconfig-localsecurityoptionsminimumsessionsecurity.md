---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07d284f778dd2cb5bfc9942a649aecbc63ac1b19
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269018"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="479f8-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="479f8-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="479f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="479f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="479f8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="479f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="479f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="479f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="479f8-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="479f8-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="479f8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="479f8-108">Members</span></span>
|<span data-ttu-id="479f8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="479f8-109">Member</span></span>|<span data-ttu-id="479f8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="479f8-110">Value</span></span>|<span data-ttu-id="479f8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="479f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="479f8-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="479f8-112">none</span></span>|<span data-ttu-id="479f8-113">,0</span><span class="sxs-lookup"><span data-stu-id="479f8-113">0</span></span>|<span data-ttu-id="479f8-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="479f8-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="479f8-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="479f8-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="479f8-116">1</span><span class="sxs-lookup"><span data-stu-id="479f8-116">1</span></span>|<span data-ttu-id="479f8-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="479f8-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="479f8-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="479f8-118">require128BitEncryption</span></span>|<span data-ttu-id="479f8-119">duas</span><span class="sxs-lookup"><span data-stu-id="479f8-119">2</span></span>|<span data-ttu-id="479f8-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="479f8-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="479f8-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="479f8-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="479f8-122">3D</span><span class="sxs-lookup"><span data-stu-id="479f8-122">3</span></span>|<span data-ttu-id="479f8-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="479f8-123">Send LM & NTLMv2 responses only</span></span>|




