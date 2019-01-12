---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a3657d60344941de931e4f77bddde922d7d01f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936358"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="12bd1-103">Cenários IVR em chamadas</span><span class="sxs-lookup"><span data-stu-id="12bd1-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="12bd1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12bd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12bd1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12bd1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12bd1-106">Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="12bd1-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="12bd1-107">Reproduzir um prompt de áudio - por exemplo, quando uma chamada é colocada na fila de um agente serviço de cliente.</span><span class="sxs-lookup"><span data-stu-id="12bd1-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="12bd1-108">Registre - por exemplo, para gravar o áudio do chamador, geralmente depois que eles ouviram um prompt com opções.</span><span class="sxs-lookup"><span data-stu-id="12bd1-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="12bd1-109">Assine o tom - por exemplo, quando você deseja saber qual DTMF toques o chamador selecionado, geralmente após ouvir o prompt de áudio.</span><span class="sxs-lookup"><span data-stu-id="12bd1-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="12bd1-110">Cancele o processamento de mídia - por exemplo, quando você deseja cancelar qualquer operação PlayPrompt ou o registro que pode ser no processo.</span><span class="sxs-lookup"><span data-stu-id="12bd1-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
