---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac7ebd94f791372b4bd7b74189204a7b8a4d0360
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989291"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="4fc4d-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4fc4d-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="4fc4d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fc4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fc4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc4d-106">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4fc4d-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="4fc4d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4fc4d-107">Members</span></span>
|<span data-ttu-id="4fc4d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4fc4d-108">Member</span></span>|<span data-ttu-id="4fc4d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4fc4d-109">Value</span></span>|<span data-ttu-id="4fc4d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fc4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc4d-111">none</span><span class="sxs-lookup"><span data-stu-id="4fc4d-111">none</span></span>|<span data-ttu-id="4fc4d-112">,0</span><span class="sxs-lookup"><span data-stu-id="4fc4d-112">0</span></span>|<span data-ttu-id="4fc4d-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4fc4d-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="4fc4d-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4fc4d-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="4fc4d-115">1</span><span class="sxs-lookup"><span data-stu-id="4fc4d-115">1</span></span>|<span data-ttu-id="4fc4d-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="4fc4d-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="4fc4d-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="4fc4d-117">require128BitEncryption</span></span>|<span data-ttu-id="4fc4d-118">duas</span><span class="sxs-lookup"><span data-stu-id="4fc4d-118">2</span></span>|<span data-ttu-id="4fc4d-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4fc4d-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="4fc4d-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="4fc4d-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="4fc4d-121">3D</span><span class="sxs-lookup"><span data-stu-id="4fc4d-121">3</span></span>|<span data-ttu-id="4fc4d-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="4fc4d-122">Send LM & NTLMv2 responses only</span></span>|





