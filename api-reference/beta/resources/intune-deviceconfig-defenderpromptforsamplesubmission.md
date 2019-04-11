---
title: tipo de enumeração defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para envio de amostras.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c81fe62d7ed2696b233b8684c665f7cf8341fbcd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778373"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="49cf7-103">tipo de enumeração defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="49cf7-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="49cf7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49cf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49cf7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49cf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cf7-106">Valores possíveis para avisar o usuário para envio de amostras.</span><span class="sxs-lookup"><span data-stu-id="49cf7-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="49cf7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="49cf7-107">Members</span></span>
|<span data-ttu-id="49cf7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="49cf7-108">Member</span></span>|<span data-ttu-id="49cf7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="49cf7-109">Value</span></span>|<span data-ttu-id="49cf7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49cf7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cf7-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="49cf7-111">userDefined</span></span>|<span data-ttu-id="49cf7-112">,0</span><span class="sxs-lookup"><span data-stu-id="49cf7-112">0</span></span>|<span data-ttu-id="49cf7-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="49cf7-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="49cf7-114">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="49cf7-114">alwaysPrompt</span></span>|<span data-ttu-id="49cf7-115">1</span><span class="sxs-lookup"><span data-stu-id="49cf7-115">1</span></span>|<span data-ttu-id="49cf7-116">Sempre avisar.</span><span class="sxs-lookup"><span data-stu-id="49cf7-116">Always prompt.</span></span>|
|<span data-ttu-id="49cf7-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="49cf7-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="49cf7-118">duas</span><span class="sxs-lookup"><span data-stu-id="49cf7-118">2</span></span>|<span data-ttu-id="49cf7-119">Avisar antes de enviar dados pessoais.</span><span class="sxs-lookup"><span data-stu-id="49cf7-119">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="49cf7-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="49cf7-120">neverSendData</span></span>|<span data-ttu-id="49cf7-121">3D</span><span class="sxs-lookup"><span data-stu-id="49cf7-121">3</span></span>|<span data-ttu-id="49cf7-122">Nunca enviar dados.</span><span class="sxs-lookup"><span data-stu-id="49cf7-122">Never send data.</span></span>|
|<span data-ttu-id="49cf7-123">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="49cf7-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="49cf7-124">quatro</span><span class="sxs-lookup"><span data-stu-id="49cf7-124">4</span></span>|<span data-ttu-id="49cf7-125">Enviar todos os dados sem avisar.</span><span class="sxs-lookup"><span data-stu-id="49cf7-125">Send all data without prompting.</span></span>|





