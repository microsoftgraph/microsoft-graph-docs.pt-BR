---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ea3267ca6c692ce916a1b8e063ac937c38618e2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802195"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="26137-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="26137-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="26137-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26137-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26137-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26137-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26137-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="26137-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="26137-107">Membros</span><span class="sxs-lookup"><span data-stu-id="26137-107">Members</span></span>
|<span data-ttu-id="26137-108">Membro</span><span class="sxs-lookup"><span data-stu-id="26137-108">Member</span></span>|<span data-ttu-id="26137-109">Valor</span><span class="sxs-lookup"><span data-stu-id="26137-109">Value</span></span>|<span data-ttu-id="26137-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26137-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26137-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="26137-111">userDefined</span></span>|<span data-ttu-id="26137-112">,0</span><span class="sxs-lookup"><span data-stu-id="26137-112">0</span></span>|<span data-ttu-id="26137-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="26137-113">Allow the user to set.</span></span>|
|<span data-ttu-id="26137-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="26137-114">none</span></span>|<span data-ttu-id="26137-115">1</span><span class="sxs-lookup"><span data-stu-id="26137-115">1</span></span>|<span data-ttu-id="26137-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="26137-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="26137-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="26137-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="26137-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="26137-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="26137-119">Basic</span><span class="sxs-lookup"><span data-stu-id="26137-119">basic</span></span>|<span data-ttu-id="26137-120">duas</span><span class="sxs-lookup"><span data-stu-id="26137-120">2</span></span>|<span data-ttu-id="26137-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="26137-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="26137-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="26137-122">enhanced</span></span>|<span data-ttu-id="26137-123">3D</span><span class="sxs-lookup"><span data-stu-id="26137-123">3</span></span>|<span data-ttu-id="26137-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="26137-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="26137-125">cheia</span><span class="sxs-lookup"><span data-stu-id="26137-125">full</span></span>|<span data-ttu-id="26137-126">quatro</span><span class="sxs-lookup"><span data-stu-id="26137-126">4</span></span>|<span data-ttu-id="26137-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="26137-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





