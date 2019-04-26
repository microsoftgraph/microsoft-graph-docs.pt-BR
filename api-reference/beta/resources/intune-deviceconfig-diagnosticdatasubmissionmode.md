---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ea3267ca6c692ce916a1b8e063ac937c38618e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567176"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="a9108-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="a9108-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="a9108-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9108-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9108-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9108-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9108-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="a9108-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="a9108-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a9108-107">Members</span></span>
|<span data-ttu-id="a9108-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a9108-108">Member</span></span>|<span data-ttu-id="a9108-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a9108-109">Value</span></span>|<span data-ttu-id="a9108-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9108-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9108-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="a9108-111">userDefined</span></span>|<span data-ttu-id="a9108-112">,0</span><span class="sxs-lookup"><span data-stu-id="a9108-112">0</span></span>|<span data-ttu-id="a9108-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="a9108-113">Allow the user to set.</span></span>|
|<span data-ttu-id="a9108-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a9108-114">none</span></span>|<span data-ttu-id="a9108-115">1 </span><span class="sxs-lookup"><span data-stu-id="a9108-115">1</span></span>|<span data-ttu-id="a9108-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="a9108-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="a9108-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="a9108-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="a9108-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="a9108-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="a9108-119">Basic</span><span class="sxs-lookup"><span data-stu-id="a9108-119">basic</span></span>|<span data-ttu-id="a9108-120">2 </span><span class="sxs-lookup"><span data-stu-id="a9108-120">2</span></span>|<span data-ttu-id="a9108-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="a9108-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="a9108-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="a9108-122">enhanced</span></span>|<span data-ttu-id="a9108-123">3 </span><span class="sxs-lookup"><span data-stu-id="a9108-123">3</span></span>|<span data-ttu-id="a9108-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="a9108-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="a9108-125">cheia</span><span class="sxs-lookup"><span data-stu-id="a9108-125">full</span></span>|<span data-ttu-id="a9108-126">4 </span><span class="sxs-lookup"><span data-stu-id="a9108-126">4</span></span>|<span data-ttu-id="a9108-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="a9108-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





