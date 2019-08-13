---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325523"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="b816d-103">tipo de enumeração localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b816d-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="b816d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b816d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b816d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b816d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b816d-106">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b816d-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="b816d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b816d-107">Members</span></span>
|<span data-ttu-id="b816d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b816d-108">Member</span></span>|<span data-ttu-id="b816d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b816d-109">Value</span></span>|<span data-ttu-id="b816d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b816d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b816d-111">none</span><span class="sxs-lookup"><span data-stu-id="b816d-111">none</span></span>|<span data-ttu-id="b816d-112">,0</span><span class="sxs-lookup"><span data-stu-id="b816d-112">0</span></span>|<span data-ttu-id="b816d-113">Enviar respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="b816d-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="b816d-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b816d-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="b816d-115">1</span><span class="sxs-lookup"><span data-stu-id="b816d-115">1</span></span>|<span data-ttu-id="b816d-116">Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada</span><span class="sxs-lookup"><span data-stu-id="b816d-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="b816d-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="b816d-117">require128BitEncryption</span></span>|<span data-ttu-id="b816d-118">duas</span><span class="sxs-lookup"><span data-stu-id="b816d-118">2</span></span>|<span data-ttu-id="b816d-119">Enviar somente respostas LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="b816d-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="b816d-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="b816d-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="b816d-121">3D</span><span class="sxs-lookup"><span data-stu-id="b816d-121">3</span></span>|<span data-ttu-id="b816d-122">Enviar somente respostas LM & NTLMv2</span><span class="sxs-lookup"><span data-stu-id="b816d-122">Send LM & NTLMv2 responses only</span></span>|



