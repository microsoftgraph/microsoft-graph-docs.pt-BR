---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da31ca3cecc74e1c74270bd34bdad14df35cc1b1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790339"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="8bc76-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8bc76-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="8bc76-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bc76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bc76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc76-106">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8bc76-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="8bc76-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8bc76-107">Members</span></span>
|<span data-ttu-id="8bc76-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8bc76-108">Member</span></span>|<span data-ttu-id="8bc76-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8bc76-109">Value</span></span>|<span data-ttu-id="8bc76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc76-111">none</span><span class="sxs-lookup"><span data-stu-id="8bc76-111">none</span></span>|<span data-ttu-id="8bc76-112">,0</span><span class="sxs-lookup"><span data-stu-id="8bc76-112">0</span></span>|<span data-ttu-id="8bc76-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="8bc76-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="8bc76-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8bc76-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="8bc76-115">1</span><span class="sxs-lookup"><span data-stu-id="8bc76-115">1</span></span>|<span data-ttu-id="8bc76-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="8bc76-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="8bc76-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8bc76-117">require128BitEncryption</span></span>|<span data-ttu-id="8bc76-118">duas</span><span class="sxs-lookup"><span data-stu-id="8bc76-118">2</span></span>|<span data-ttu-id="8bc76-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="8bc76-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="8bc76-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8bc76-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="8bc76-121">3D</span><span class="sxs-lookup"><span data-stu-id="8bc76-121">3</span></span>|<span data-ttu-id="8bc76-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="8bc76-122">Send LM & NTLMv2 responses only</span></span>|



