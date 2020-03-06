---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 838f90e8396be1ae3a55ea28f749cfd5b42edd01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532550"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="39af5-103">tipo de enumeração diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="39af5-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="39af5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39af5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39af5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39af5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39af5-106">Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="39af5-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="39af5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="39af5-107">Members</span></span>
|<span data-ttu-id="39af5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="39af5-108">Member</span></span>|<span data-ttu-id="39af5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="39af5-109">Value</span></span>|<span data-ttu-id="39af5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39af5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39af5-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="39af5-111">userDefined</span></span>|<span data-ttu-id="39af5-112">,0</span><span class="sxs-lookup"><span data-stu-id="39af5-112">0</span></span>|<span data-ttu-id="39af5-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="39af5-113">Allow the user to set.</span></span>|
|<span data-ttu-id="39af5-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="39af5-114">none</span></span>|<span data-ttu-id="39af5-115">1 </span><span class="sxs-lookup"><span data-stu-id="39af5-115">1</span></span>|<span data-ttu-id="39af5-116">Nenhum dado de telemetria é enviado dos componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="39af5-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="39af5-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="39af5-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="39af5-118">O uso dessa configuração em outros dispositivos equivale a definir o valor 1.</span><span class="sxs-lookup"><span data-stu-id="39af5-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="39af5-119">Basic</span><span class="sxs-lookup"><span data-stu-id="39af5-119">basic</span></span>|<span data-ttu-id="39af5-120">2 </span><span class="sxs-lookup"><span data-stu-id="39af5-120">2</span></span>|<span data-ttu-id="39af5-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="39af5-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="39af5-122">metarquivo</span><span class="sxs-lookup"><span data-stu-id="39af5-122">enhanced</span></span>|<span data-ttu-id="39af5-123">3 </span><span class="sxs-lookup"><span data-stu-id="39af5-123">3</span></span>|<span data-ttu-id="39af5-124">Envia dados de telemetria avançados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="39af5-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="39af5-125">cheia</span><span class="sxs-lookup"><span data-stu-id="39af5-125">full</span></span>|<span data-ttu-id="39af5-126">4 </span><span class="sxs-lookup"><span data-stu-id="39af5-126">4</span></span>|<span data-ttu-id="39af5-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="39af5-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




