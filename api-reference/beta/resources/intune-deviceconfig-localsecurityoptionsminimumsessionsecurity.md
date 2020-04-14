---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f5d7e052d5b814bb10d3c0851683deccdf9f9f5f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439970"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="5bbf1-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5bbf1-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="5bbf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bbf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bbf1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5bbf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bbf1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bbf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bbf1-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5bbf1-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="5bbf1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5bbf1-108">Members</span></span>
|<span data-ttu-id="5bbf1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5bbf1-109">Member</span></span>|<span data-ttu-id="5bbf1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5bbf1-110">Value</span></span>|<span data-ttu-id="5bbf1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bbf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bbf1-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="5bbf1-112">none</span></span>|<span data-ttu-id="5bbf1-113">,0</span><span class="sxs-lookup"><span data-stu-id="5bbf1-113">0</span></span>|<span data-ttu-id="5bbf1-114">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="5bbf1-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="5bbf1-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5bbf1-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="5bbf1-116">1</span><span class="sxs-lookup"><span data-stu-id="5bbf1-116">1</span></span>|<span data-ttu-id="5bbf1-117">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="5bbf1-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="5bbf1-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5bbf1-118">require128BitEncryption</span></span>|<span data-ttu-id="5bbf1-119">duas</span><span class="sxs-lookup"><span data-stu-id="5bbf1-119">2</span></span>|<span data-ttu-id="5bbf1-120">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="5bbf1-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="5bbf1-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5bbf1-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="5bbf1-122">3D</span><span class="sxs-lookup"><span data-stu-id="5bbf1-122">3</span></span>|<span data-ttu-id="5bbf1-123">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="5bbf1-123">Send LM & NTLMv2 responses only</span></span>|



