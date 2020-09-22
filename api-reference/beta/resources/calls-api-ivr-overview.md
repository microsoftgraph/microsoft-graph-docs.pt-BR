---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 3b33a673218238f861e7122de8320d6c8a20e435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042727"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="77fe1-103">Cenários IVR em chamadas</span><span class="sxs-lookup"><span data-stu-id="77fe1-103">IVR scenarios in calls</span></span>

<span data-ttu-id="77fe1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77fe1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77fe1-105">Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:</span><span class="sxs-lookup"><span data-stu-id="77fe1-105">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="77fe1-106">Reproduzir um prompt de áudio-por exemplo, quando uma chamada é colocada em uma fila de agente de atendimento ao cliente.</span><span class="sxs-lookup"><span data-stu-id="77fe1-106">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="77fe1-107">Gravar uma resposta-por exemplo, para registrar o áudio do chamador, normalmente após ouvir um prompt com as opções.</span><span class="sxs-lookup"><span data-stu-id="77fe1-107">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="77fe1-108">Inscrever-se em tons-por exemplo, quando você deseja saber quais tons de DTMF o chamador selecionou, geralmente após ouvir o prompt de áudio.</span><span class="sxs-lookup"><span data-stu-id="77fe1-108">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="77fe1-109">Cancelar o processamento de mídia – por exemplo, quando você deseja cancelar qualquer operação do playPrompt ou do recordResponse que possa estar em processo.</span><span class="sxs-lookup"><span data-stu-id="77fe1-109">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>


