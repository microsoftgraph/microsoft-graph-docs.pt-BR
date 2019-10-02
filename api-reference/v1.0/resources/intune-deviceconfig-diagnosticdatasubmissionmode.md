---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 15abccb0bf2171e62c2b468ecf5c3078e052ea75
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359373"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="3e8f7-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="3e8f7-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="3e8f7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e8f7-105">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="3e8f7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="3e8f7-106">Members</span></span>
|<span data-ttu-id="3e8f7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="3e8f7-107">Member</span></span>|<span data-ttu-id="3e8f7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="3e8f7-108">Value</span></span>|<span data-ttu-id="3e8f7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e8f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8f7-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="3e8f7-110">userDefined</span></span>|<span data-ttu-id="3e8f7-111">,0</span><span class="sxs-lookup"><span data-stu-id="3e8f7-111">0</span></span>|<span data-ttu-id="3e8f7-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-112">Allow the user to set.</span></span>|
|<span data-ttu-id="3e8f7-113">none</span><span class="sxs-lookup"><span data-stu-id="3e8f7-113">none</span></span>|<span data-ttu-id="3e8f7-114">1</span><span class="sxs-lookup"><span data-stu-id="3e8f7-114">1</span></span>|<span data-ttu-id="3e8f7-115">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="3e8f7-116">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="3e8f7-117">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="3e8f7-118">Basic</span><span class="sxs-lookup"><span data-stu-id="3e8f7-118">basic</span></span>|<span data-ttu-id="3e8f7-119">duas</span><span class="sxs-lookup"><span data-stu-id="3e8f7-119">2</span></span>|<span data-ttu-id="3e8f7-120">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="3e8f7-121">metarquivo</span><span class="sxs-lookup"><span data-stu-id="3e8f7-121">enhanced</span></span>|<span data-ttu-id="3e8f7-122">3D</span><span class="sxs-lookup"><span data-stu-id="3e8f7-122">3</span></span>|<span data-ttu-id="3e8f7-123">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="3e8f7-124">cheia</span><span class="sxs-lookup"><span data-stu-id="3e8f7-124">full</span></span>|<span data-ttu-id="3e8f7-125">quatro</span><span class="sxs-lookup"><span data-stu-id="3e8f7-125">4</span></span>|<span data-ttu-id="3e8f7-126">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="3e8f7-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




