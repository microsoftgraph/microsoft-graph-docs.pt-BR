---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578019"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="caa52-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="caa52-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="caa52-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="caa52-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caa52-105">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="caa52-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="caa52-106">Membros</span><span class="sxs-lookup"><span data-stu-id="caa52-106">Members</span></span>
|<span data-ttu-id="caa52-107">Membro</span><span class="sxs-lookup"><span data-stu-id="caa52-107">Member</span></span>|<span data-ttu-id="caa52-108">Valor</span><span class="sxs-lookup"><span data-stu-id="caa52-108">Value</span></span>|<span data-ttu-id="caa52-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="caa52-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caa52-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="caa52-110">userDefined</span></span>|<span data-ttu-id="caa52-111">,0</span><span class="sxs-lookup"><span data-stu-id="caa52-111">0</span></span>|<span data-ttu-id="caa52-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="caa52-112">Allow the user to set.</span></span>|
|<span data-ttu-id="caa52-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="caa52-113">none</span></span>|<span data-ttu-id="caa52-114">1 </span><span class="sxs-lookup"><span data-stu-id="caa52-114">1</span></span>|<span data-ttu-id="caa52-115">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="caa52-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="caa52-116">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="caa52-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="caa52-117">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="caa52-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="caa52-118">Basic</span><span class="sxs-lookup"><span data-stu-id="caa52-118">basic</span></span>|<span data-ttu-id="caa52-119">2 </span><span class="sxs-lookup"><span data-stu-id="caa52-119">2</span></span>|<span data-ttu-id="caa52-120">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="caa52-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="caa52-121">metarquivo</span><span class="sxs-lookup"><span data-stu-id="caa52-121">enhanced</span></span>|<span data-ttu-id="caa52-122">3 </span><span class="sxs-lookup"><span data-stu-id="caa52-122">3</span></span>|<span data-ttu-id="caa52-123">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="caa52-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="caa52-124">cheia</span><span class="sxs-lookup"><span data-stu-id="caa52-124">full</span></span>|<span data-ttu-id="caa52-125">4 </span><span class="sxs-lookup"><span data-stu-id="caa52-125">4</span></span>|<span data-ttu-id="caa52-126">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="caa52-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



