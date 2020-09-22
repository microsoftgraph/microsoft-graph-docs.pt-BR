---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e85544eef7556fd70c880f9c402966d251da6fc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056818"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="fe9c4-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="fe9c4-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="fe9c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe9c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe9c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe9c4-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="fe9c4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fe9c4-107">Members</span></span>
|<span data-ttu-id="fe9c4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fe9c4-108">Member</span></span>|<span data-ttu-id="fe9c4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fe9c4-109">Value</span></span>|<span data-ttu-id="fe9c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe9c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe9c4-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="fe9c4-111">userDefined</span></span>|<span data-ttu-id="fe9c4-112">,0</span><span class="sxs-lookup"><span data-stu-id="fe9c4-112">0</span></span>|<span data-ttu-id="fe9c4-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-113">Allow the user to set.</span></span>|
|<span data-ttu-id="fe9c4-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fe9c4-114">none</span></span>|<span data-ttu-id="fe9c4-115">1 </span><span class="sxs-lookup"><span data-stu-id="fe9c4-115">1</span></span>|<span data-ttu-id="fe9c4-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="fe9c4-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="fe9c4-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="fe9c4-119">Basic</span><span class="sxs-lookup"><span data-stu-id="fe9c4-119">basic</span></span>|<span data-ttu-id="fe9c4-120">2 </span><span class="sxs-lookup"><span data-stu-id="fe9c4-120">2</span></span>|<span data-ttu-id="fe9c4-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="fe9c4-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="fe9c4-122">enhanced</span></span>|<span data-ttu-id="fe9c4-123">3 </span><span class="sxs-lookup"><span data-stu-id="fe9c4-123">3</span></span>|<span data-ttu-id="fe9c4-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="fe9c4-125">cheia</span><span class="sxs-lookup"><span data-stu-id="fe9c4-125">full</span></span>|<span data-ttu-id="fe9c4-126">4 </span><span class="sxs-lookup"><span data-stu-id="fe9c4-126">4</span></span>|<span data-ttu-id="fe9c4-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="fe9c4-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|









