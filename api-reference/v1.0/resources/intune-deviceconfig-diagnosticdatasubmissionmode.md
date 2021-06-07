---
title: tipo denum diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 172ac80e4491d238414777c4d1d30d9f969f2a39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755081"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="4ad34-103">tipo denum diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="4ad34-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="4ad34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ad34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ad34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ad34-106">Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="4ad34-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="4ad34-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4ad34-107">Members</span></span>
|<span data-ttu-id="4ad34-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4ad34-108">Member</span></span>|<span data-ttu-id="4ad34-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4ad34-109">Value</span></span>|<span data-ttu-id="4ad34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad34-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="4ad34-111">userDefined</span></span>|<span data-ttu-id="4ad34-112">0</span><span class="sxs-lookup"><span data-stu-id="4ad34-112">0</span></span>|<span data-ttu-id="4ad34-113">Permitir que o usuário desem conjunto.</span><span class="sxs-lookup"><span data-stu-id="4ad34-113">Allow the user to set.</span></span>|
|<span data-ttu-id="4ad34-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="4ad34-114">none</span></span>|<span data-ttu-id="4ad34-115">1</span><span class="sxs-lookup"><span data-stu-id="4ad34-115">1</span></span>|<span data-ttu-id="4ad34-116">Nenhum dado de telemetria é enviado de componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4ad34-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="4ad34-117">Observação: esse valor só é aplicável a dispositivos corporativos e de servidor.</span><span class="sxs-lookup"><span data-stu-id="4ad34-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="4ad34-118">Usar essa configuração em outros dispositivos é equivalente à definição do valor 1.</span><span class="sxs-lookup"><span data-stu-id="4ad34-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="4ad34-119">basic</span><span class="sxs-lookup"><span data-stu-id="4ad34-119">basic</span></span>|<span data-ttu-id="4ad34-120">2</span><span class="sxs-lookup"><span data-stu-id="4ad34-120">2</span></span>|<span data-ttu-id="4ad34-121">Envia dados básicos de telemetria.</span><span class="sxs-lookup"><span data-stu-id="4ad34-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="4ad34-122">enhanced</span><span class="sxs-lookup"><span data-stu-id="4ad34-122">enhanced</span></span>|<span data-ttu-id="4ad34-123">3</span><span class="sxs-lookup"><span data-stu-id="4ad34-123">3</span></span>|<span data-ttu-id="4ad34-124">Envia dados de telemetria aprimorados, incluindo dados de uso e insights.</span><span class="sxs-lookup"><span data-stu-id="4ad34-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="4ad34-125">full</span><span class="sxs-lookup"><span data-stu-id="4ad34-125">full</span></span>|<span data-ttu-id="4ad34-126">4 </span><span class="sxs-lookup"><span data-stu-id="4ad34-126">4</span></span>|<span data-ttu-id="4ad34-127">Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="4ad34-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




