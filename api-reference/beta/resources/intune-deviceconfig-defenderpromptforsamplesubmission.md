---
title: tipo de enum defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para amostras de envio.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8dfc1a3aeb80a22041f799fb40ff9b2cc6e3870b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924822"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="da60b-103">tipo de enum defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="da60b-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="da60b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da60b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da60b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da60b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da60b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da60b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da60b-107">Valores possíveis para avisar o usuário para amostras de envio.</span><span class="sxs-lookup"><span data-stu-id="da60b-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="da60b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="da60b-108">Members</span></span>
|<span data-ttu-id="da60b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="da60b-109">Member</span></span>|<span data-ttu-id="da60b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="da60b-110">Value</span></span>|<span data-ttu-id="da60b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da60b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da60b-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="da60b-112">userDefined</span></span>|<span data-ttu-id="da60b-113">0</span><span class="sxs-lookup"><span data-stu-id="da60b-113">0</span></span>|<span data-ttu-id="da60b-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="da60b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="da60b-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="da60b-115">alwaysPrompt</span></span>|<span data-ttu-id="da60b-116">1</span><span class="sxs-lookup"><span data-stu-id="da60b-116">1</span></span>|<span data-ttu-id="da60b-117">Sempre avisar.</span><span class="sxs-lookup"><span data-stu-id="da60b-117">Always prompt.</span></span>|
|<span data-ttu-id="da60b-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="da60b-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="da60b-119">2</span><span class="sxs-lookup"><span data-stu-id="da60b-119">2</span></span>|<span data-ttu-id="da60b-120">Avisar antes de enviar dados pessoais.</span><span class="sxs-lookup"><span data-stu-id="da60b-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="da60b-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="da60b-121">neverSendData</span></span>|<span data-ttu-id="da60b-122">3</span><span class="sxs-lookup"><span data-stu-id="da60b-122">3</span></span>|<span data-ttu-id="da60b-123">Nunca envie dados.</span><span class="sxs-lookup"><span data-stu-id="da60b-123">Never send data.</span></span>|
|<span data-ttu-id="da60b-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="da60b-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="da60b-125">4</span><span class="sxs-lookup"><span data-stu-id="da60b-125">4</span></span>|<span data-ttu-id="da60b-126">Envie todos os dados sem avisar.</span><span class="sxs-lookup"><span data-stu-id="da60b-126">Send all data without prompting.</span></span>|





