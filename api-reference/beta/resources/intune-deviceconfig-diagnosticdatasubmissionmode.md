---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf69232ee31bf7fd1eebd440e482d76c052f4fbc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989921"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="c9def-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="c9def-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="c9def-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9def-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9def-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9def-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9def-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="c9def-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="c9def-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c9def-107">Members</span></span>
|<span data-ttu-id="c9def-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c9def-108">Member</span></span>|<span data-ttu-id="c9def-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c9def-109">Value</span></span>|<span data-ttu-id="c9def-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9def-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9def-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="c9def-111">userDefined</span></span>|<span data-ttu-id="c9def-112">,0</span><span class="sxs-lookup"><span data-stu-id="c9def-112">0</span></span>|<span data-ttu-id="c9def-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="c9def-113">Allow the user to set.</span></span>|
|<span data-ttu-id="c9def-114">none</span><span class="sxs-lookup"><span data-stu-id="c9def-114">none</span></span>|<span data-ttu-id="c9def-115">1</span><span class="sxs-lookup"><span data-stu-id="c9def-115">1</span></span>|<span data-ttu-id="c9def-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c9def-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="c9def-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="c9def-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="c9def-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="c9def-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="c9def-119">Basic</span><span class="sxs-lookup"><span data-stu-id="c9def-119">basic</span></span>|<span data-ttu-id="c9def-120">duas</span><span class="sxs-lookup"><span data-stu-id="c9def-120">2</span></span>|<span data-ttu-id="c9def-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="c9def-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="c9def-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="c9def-122">enhanced</span></span>|<span data-ttu-id="c9def-123">3D</span><span class="sxs-lookup"><span data-stu-id="c9def-123">3</span></span>|<span data-ttu-id="c9def-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="c9def-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="c9def-125">cheia</span><span class="sxs-lookup"><span data-stu-id="c9def-125">full</span></span>|<span data-ttu-id="c9def-126">quatro</span><span class="sxs-lookup"><span data-stu-id="c9def-126">4</span></span>|<span data-ttu-id="c9def-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="c9def-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





