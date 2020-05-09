---
title: tipo de enumeração defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para envio de amostras.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d5cf699b386dbf0c6d75a19522529386ab36977d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177699"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="26d61-103">tipo de enumeração defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="26d61-103">defenderPromptForSampleSubmission enum type</span></span>

<span data-ttu-id="26d61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26d61-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26d61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26d61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26d61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26d61-107">Valores possíveis para avisar o usuário para envio de amostras.</span><span class="sxs-lookup"><span data-stu-id="26d61-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="26d61-108">Membros</span><span class="sxs-lookup"><span data-stu-id="26d61-108">Members</span></span>
|<span data-ttu-id="26d61-109">Membro</span><span class="sxs-lookup"><span data-stu-id="26d61-109">Member</span></span>|<span data-ttu-id="26d61-110">Valor</span><span class="sxs-lookup"><span data-stu-id="26d61-110">Value</span></span>|<span data-ttu-id="26d61-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d61-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="26d61-112">userDefined</span></span>|<span data-ttu-id="26d61-113">,0</span><span class="sxs-lookup"><span data-stu-id="26d61-113">0</span></span>|<span data-ttu-id="26d61-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="26d61-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="26d61-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="26d61-115">alwaysPrompt</span></span>|<span data-ttu-id="26d61-116">1</span><span class="sxs-lookup"><span data-stu-id="26d61-116">1</span></span>|<span data-ttu-id="26d61-117">Sempre avisar.</span><span class="sxs-lookup"><span data-stu-id="26d61-117">Always prompt.</span></span>|
|<span data-ttu-id="26d61-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="26d61-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="26d61-119">duas</span><span class="sxs-lookup"><span data-stu-id="26d61-119">2</span></span>|<span data-ttu-id="26d61-120">Enviar amostras seguras automaticamente.</span><span class="sxs-lookup"><span data-stu-id="26d61-120">Send safe samples automatically.</span></span>|
|<span data-ttu-id="26d61-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="26d61-121">neverSendData</span></span>|<span data-ttu-id="26d61-122">3D</span><span class="sxs-lookup"><span data-stu-id="26d61-122">3</span></span>|<span data-ttu-id="26d61-123">Nunca enviar dados.</span><span class="sxs-lookup"><span data-stu-id="26d61-123">Never send data.</span></span>|
|<span data-ttu-id="26d61-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="26d61-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="26d61-125">4 </span><span class="sxs-lookup"><span data-stu-id="26d61-125">4</span></span>|<span data-ttu-id="26d61-126">Enviar todos os dados sem avisar.</span><span class="sxs-lookup"><span data-stu-id="26d61-126">Send all data without prompting.</span></span>|



