---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e749d2fc7a1eb191c62fbc9db389887cdd901c27
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175217"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="c0404-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="c0404-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="c0404-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0404-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0404-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0404-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0404-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="c0404-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="c0404-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c0404-107">Members</span></span>
|<span data-ttu-id="c0404-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c0404-108">Member</span></span>|<span data-ttu-id="c0404-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c0404-109">Value</span></span>|<span data-ttu-id="c0404-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0404-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0404-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="c0404-111">userDefined</span></span>|<span data-ttu-id="c0404-112">,0</span><span class="sxs-lookup"><span data-stu-id="c0404-112">0</span></span>|<span data-ttu-id="c0404-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="c0404-113">Allow the user to set.</span></span>|
|<span data-ttu-id="c0404-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c0404-114">none</span></span>|<span data-ttu-id="c0404-115">1</span><span class="sxs-lookup"><span data-stu-id="c0404-115">1</span></span>|<span data-ttu-id="c0404-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c0404-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="c0404-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="c0404-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="c0404-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="c0404-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="c0404-119">Basic</span><span class="sxs-lookup"><span data-stu-id="c0404-119">basic</span></span>|<span data-ttu-id="c0404-120">duas</span><span class="sxs-lookup"><span data-stu-id="c0404-120">2</span></span>|<span data-ttu-id="c0404-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="c0404-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="c0404-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="c0404-122">enhanced</span></span>|<span data-ttu-id="c0404-123">3D</span><span class="sxs-lookup"><span data-stu-id="c0404-123">3</span></span>|<span data-ttu-id="c0404-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="c0404-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="c0404-125">cheia</span><span class="sxs-lookup"><span data-stu-id="c0404-125">full</span></span>|<span data-ttu-id="c0404-126">quatro</span><span class="sxs-lookup"><span data-stu-id="c0404-126">4</span></span>|<span data-ttu-id="c0404-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="c0404-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




