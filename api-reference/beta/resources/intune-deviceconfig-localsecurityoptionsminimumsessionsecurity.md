---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396081"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="68f26-103">tipo de enum localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="68f26-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="68f26-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="68f26-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68f26-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68f26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68f26-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="68f26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f26-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="68f26-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="68f26-108">Membros</span><span class="sxs-lookup"><span data-stu-id="68f26-108">Members</span></span>
|<span data-ttu-id="68f26-109">Membro</span><span class="sxs-lookup"><span data-stu-id="68f26-109">Member</span></span>|<span data-ttu-id="68f26-110">Valor</span><span class="sxs-lookup"><span data-stu-id="68f26-110">Value</span></span>|<span data-ttu-id="68f26-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68f26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f26-112">none</span><span class="sxs-lookup"><span data-stu-id="68f26-112">none</span></span>|<span data-ttu-id="68f26-113">0</span><span class="sxs-lookup"><span data-stu-id="68f26-113">0</span></span>|<span data-ttu-id="68f26-114">Enviar LM & respostas NTLM</span><span class="sxs-lookup"><span data-stu-id="68f26-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="68f26-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="68f26-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="68f26-116">1</span><span class="sxs-lookup"><span data-stu-id="68f26-116">1</span></span>|<span data-ttu-id="68f26-117">Enviar a segurança da sessão do LM & usar NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="68f26-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="68f26-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="68f26-118">require128BitEncryption</span></span>|<span data-ttu-id="68f26-119">2</span><span class="sxs-lookup"><span data-stu-id="68f26-119">2</span></span>|<span data-ttu-id="68f26-120">Enviar LM & somente respostas NTLM</span><span class="sxs-lookup"><span data-stu-id="68f26-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="68f26-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="68f26-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="68f26-122">3</span><span class="sxs-lookup"><span data-stu-id="68f26-122">3</span></span>|<span data-ttu-id="68f26-123">Enviar LM & respostas NTLMv2</span><span class="sxs-lookup"><span data-stu-id="68f26-123">Send LM & NTLMv2 responses only</span></span>|




