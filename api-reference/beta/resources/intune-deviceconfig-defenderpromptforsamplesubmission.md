---
title: tipo de enumeração defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para envio de amostras.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ee46596bd6d9f788f39afd0d3628f27acebf69b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073772"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="92e7b-103">tipo de enumeração defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="92e7b-103">defenderPromptForSampleSubmission enum type</span></span>

<span data-ttu-id="92e7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92e7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92e7b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92e7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e7b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92e7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e7b-107">Valores possíveis para avisar o usuário para envio de amostras.</span><span class="sxs-lookup"><span data-stu-id="92e7b-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="92e7b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="92e7b-108">Members</span></span>
|<span data-ttu-id="92e7b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="92e7b-109">Member</span></span>|<span data-ttu-id="92e7b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="92e7b-110">Value</span></span>|<span data-ttu-id="92e7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="92e7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e7b-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="92e7b-112">userDefined</span></span>|<span data-ttu-id="92e7b-113">,0</span><span class="sxs-lookup"><span data-stu-id="92e7b-113">0</span></span>|<span data-ttu-id="92e7b-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="92e7b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="92e7b-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="92e7b-115">alwaysPrompt</span></span>|<span data-ttu-id="92e7b-116">1 </span><span class="sxs-lookup"><span data-stu-id="92e7b-116">1</span></span>|<span data-ttu-id="92e7b-117">Sempre avisar.</span><span class="sxs-lookup"><span data-stu-id="92e7b-117">Always prompt.</span></span>|
|<span data-ttu-id="92e7b-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="92e7b-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="92e7b-119">2 </span><span class="sxs-lookup"><span data-stu-id="92e7b-119">2</span></span>|<span data-ttu-id="92e7b-120">Enviar amostras seguras automaticamente.</span><span class="sxs-lookup"><span data-stu-id="92e7b-120">Send safe samples automatically.</span></span>|
|<span data-ttu-id="92e7b-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="92e7b-121">neverSendData</span></span>|<span data-ttu-id="92e7b-122">3 </span><span class="sxs-lookup"><span data-stu-id="92e7b-122">3</span></span>|<span data-ttu-id="92e7b-123">Nunca enviar dados.</span><span class="sxs-lookup"><span data-stu-id="92e7b-123">Never send data.</span></span>|
|<span data-ttu-id="92e7b-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="92e7b-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="92e7b-125">4 </span><span class="sxs-lookup"><span data-stu-id="92e7b-125">4</span></span>|<span data-ttu-id="92e7b-126">Enviar todos os dados sem avisar.</span><span class="sxs-lookup"><span data-stu-id="92e7b-126">Send all data without prompting.</span></span>|






