---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 2b9d4b26d121c7abef1b677db7490a8ec03386c9
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439945"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="560fc-103">Cenários IVR em chamadas</span><span class="sxs-lookup"><span data-stu-id="560fc-103">IVR scenarios in calls</span></span>

<span data-ttu-id="560fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="560fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="560fc-105">Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:</span><span class="sxs-lookup"><span data-stu-id="560fc-105">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="560fc-106">Reproduzir um prompt de áudio-por exemplo, quando uma chamada é colocada em uma fila de agente de atendimento ao cliente.</span><span class="sxs-lookup"><span data-stu-id="560fc-106">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="560fc-107">Gravar uma resposta-por exemplo, para registrar o áudio do chamador, normalmente após ouvir um prompt com as opções.</span><span class="sxs-lookup"><span data-stu-id="560fc-107">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="560fc-108">Inscrever-se em tons-por exemplo, quando você deseja saber quais tons de DTMF o chamador selecionou, geralmente após ouvir o prompt de áudio.</span><span class="sxs-lookup"><span data-stu-id="560fc-108">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="560fc-109">Cancelar o processamento de mídia – por exemplo, quando você deseja cancelar qualquer operação do playPrompt ou do recordResponse que possa estar em processo.</span><span class="sxs-lookup"><span data-stu-id="560fc-109">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>
