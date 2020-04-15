---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 80a936c103caa4655addd25f8a21d75d9bc67040
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465685"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="c586b-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="c586b-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="c586b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c586b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c586b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c586b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c586b-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="c586b-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="c586b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c586b-107">Members</span></span>
|<span data-ttu-id="c586b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c586b-108">Member</span></span>|<span data-ttu-id="c586b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c586b-109">Value</span></span>|<span data-ttu-id="c586b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c586b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c586b-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="c586b-111">userDefined</span></span>|<span data-ttu-id="c586b-112">,0</span><span class="sxs-lookup"><span data-stu-id="c586b-112">0</span></span>|<span data-ttu-id="c586b-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="c586b-113">Allow the user to set.</span></span>|
|<span data-ttu-id="c586b-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="c586b-114">none</span></span>|<span data-ttu-id="c586b-115">1</span><span class="sxs-lookup"><span data-stu-id="c586b-115">1</span></span>|<span data-ttu-id="c586b-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c586b-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="c586b-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="c586b-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="c586b-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="c586b-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="c586b-119">Basic</span><span class="sxs-lookup"><span data-stu-id="c586b-119">basic</span></span>|<span data-ttu-id="c586b-120">duas</span><span class="sxs-lookup"><span data-stu-id="c586b-120">2</span></span>|<span data-ttu-id="c586b-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="c586b-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="c586b-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="c586b-122">enhanced</span></span>|<span data-ttu-id="c586b-123">3D</span><span class="sxs-lookup"><span data-stu-id="c586b-123">3</span></span>|<span data-ttu-id="c586b-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="c586b-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="c586b-125">cheia</span><span class="sxs-lookup"><span data-stu-id="c586b-125">full</span></span>|<span data-ttu-id="c586b-126">4 </span><span class="sxs-lookup"><span data-stu-id="c586b-126">4</span></span>|<span data-ttu-id="c586b-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="c586b-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|







