---
title: tipo de enumeração defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para envio de amostras.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37d585e11a539724e57a99d63673f076bc5f4f11
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256425"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="a2f20-103">tipo de enumeração defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="a2f20-103">defenderPromptForSampleSubmission enum type</span></span>

<span data-ttu-id="a2f20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2f20-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2f20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2f20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2f20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2f20-107">Valores possíveis para avisar o usuário para envio de amostras.</span><span class="sxs-lookup"><span data-stu-id="a2f20-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="a2f20-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a2f20-108">Members</span></span>
|<span data-ttu-id="a2f20-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a2f20-109">Member</span></span>|<span data-ttu-id="a2f20-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a2f20-110">Value</span></span>|<span data-ttu-id="a2f20-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2f20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f20-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="a2f20-112">userDefined</span></span>|<span data-ttu-id="a2f20-113">,0</span><span class="sxs-lookup"><span data-stu-id="a2f20-113">0</span></span>|<span data-ttu-id="a2f20-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a2f20-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a2f20-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="a2f20-115">alwaysPrompt</span></span>|<span data-ttu-id="a2f20-116">1</span><span class="sxs-lookup"><span data-stu-id="a2f20-116">1</span></span>|<span data-ttu-id="a2f20-117">Sempre avisar.</span><span class="sxs-lookup"><span data-stu-id="a2f20-117">Always prompt.</span></span>|
|<span data-ttu-id="a2f20-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="a2f20-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="a2f20-119">duas</span><span class="sxs-lookup"><span data-stu-id="a2f20-119">2</span></span>|<span data-ttu-id="a2f20-120">Enviar amostras seguras automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a2f20-120">Send safe samples automatically.</span></span>|
|<span data-ttu-id="a2f20-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="a2f20-121">neverSendData</span></span>|<span data-ttu-id="a2f20-122">3D</span><span class="sxs-lookup"><span data-stu-id="a2f20-122">3</span></span>|<span data-ttu-id="a2f20-123">Nunca enviar dados.</span><span class="sxs-lookup"><span data-stu-id="a2f20-123">Never send data.</span></span>|
|<span data-ttu-id="a2f20-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="a2f20-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="a2f20-125">4 </span><span class="sxs-lookup"><span data-stu-id="a2f20-125">4</span></span>|<span data-ttu-id="a2f20-126">Enviar todos os dados sem avisar.</span><span class="sxs-lookup"><span data-stu-id="a2f20-126">Send all data without prompting.</span></span>|




