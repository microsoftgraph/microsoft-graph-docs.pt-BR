---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350628"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="95d18-103">tipo de enum localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="95d18-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="95d18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95d18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95d18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95d18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95d18-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="95d18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95d18-107">Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="95d18-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="95d18-108">Membros</span><span class="sxs-lookup"><span data-stu-id="95d18-108">Members</span></span>
|<span data-ttu-id="95d18-109">Membro</span><span class="sxs-lookup"><span data-stu-id="95d18-109">Member</span></span>|<span data-ttu-id="95d18-110">Valor</span><span class="sxs-lookup"><span data-stu-id="95d18-110">Value</span></span>|<span data-ttu-id="95d18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="95d18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95d18-112">none</span><span class="sxs-lookup"><span data-stu-id="95d18-112">none</span></span>|<span data-ttu-id="95d18-113">0</span><span class="sxs-lookup"><span data-stu-id="95d18-113">0</span></span>|<span data-ttu-id="95d18-114">Enviar respostas LM e NTLM</span><span class="sxs-lookup"><span data-stu-id="95d18-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="95d18-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="95d18-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="95d18-116">1</span><span class="sxs-lookup"><span data-stu-id="95d18-116">1</span></span>|<span data-ttu-id="95d18-117">Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado</span><span class="sxs-lookup"><span data-stu-id="95d18-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="95d18-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="95d18-118">require128BitEncryption</span></span>|<span data-ttu-id="95d18-119">2</span><span class="sxs-lookup"><span data-stu-id="95d18-119">2</span></span>|<span data-ttu-id="95d18-120">Enviar respostas LM & NTLM somente</span><span class="sxs-lookup"><span data-stu-id="95d18-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="95d18-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="95d18-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="95d18-122">3</span><span class="sxs-lookup"><span data-stu-id="95d18-122">3</span></span>|<span data-ttu-id="95d18-123">Enviar respostas LM & NTLMv2 somente</span><span class="sxs-lookup"><span data-stu-id="95d18-123">Send LM & NTLMv2 responses only</span></span>|





