---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ef0a61e8d95793e6e4717a3a5ed66d518e80590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968441"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="28928-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="28928-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="28928-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28928-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28928-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28928-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28928-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28928-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28928-107">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="28928-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="28928-108">Membros</span><span class="sxs-lookup"><span data-stu-id="28928-108">Members</span></span>
|<span data-ttu-id="28928-109">Membro</span><span class="sxs-lookup"><span data-stu-id="28928-109">Member</span></span>|<span data-ttu-id="28928-110">Valor</span><span class="sxs-lookup"><span data-stu-id="28928-110">Value</span></span>|<span data-ttu-id="28928-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28928-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28928-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="28928-112">userDefined</span></span>|<span data-ttu-id="28928-113">,0</span><span class="sxs-lookup"><span data-stu-id="28928-113">0</span></span>|<span data-ttu-id="28928-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="28928-114">Allow the user to set.</span></span>|
|<span data-ttu-id="28928-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="28928-115">none</span></span>|<span data-ttu-id="28928-116">1 </span><span class="sxs-lookup"><span data-stu-id="28928-116">1</span></span>|<span data-ttu-id="28928-117">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="28928-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="28928-118">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="28928-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="28928-119">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="28928-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="28928-120">Basic</span><span class="sxs-lookup"><span data-stu-id="28928-120">basic</span></span>|<span data-ttu-id="28928-121">2 </span><span class="sxs-lookup"><span data-stu-id="28928-121">2</span></span>|<span data-ttu-id="28928-122">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="28928-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="28928-123">metarquivo</span><span class="sxs-lookup"><span data-stu-id="28928-123">enhanced</span></span>|<span data-ttu-id="28928-124">3 </span><span class="sxs-lookup"><span data-stu-id="28928-124">3</span></span>|<span data-ttu-id="28928-125">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="28928-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="28928-126">cheia</span><span class="sxs-lookup"><span data-stu-id="28928-126">full</span></span>|<span data-ttu-id="28928-127">4 </span><span class="sxs-lookup"><span data-stu-id="28928-127">4</span></span>|<span data-ttu-id="28928-128">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="28928-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|






