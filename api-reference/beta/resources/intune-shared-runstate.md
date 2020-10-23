---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ec8d3f9333393b946539d639c9cc9eeb30c6b027
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725152"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="27b35-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="27b35-103">runState enum type</span></span>

<span data-ttu-id="27b35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27b35-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27b35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27b35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27b35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27b35-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27b35-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="27b35-108">Membros</span><span class="sxs-lookup"><span data-stu-id="27b35-108">Members</span></span>
|<span data-ttu-id="27b35-109">Membro</span><span class="sxs-lookup"><span data-stu-id="27b35-109">Member</span></span>|<span data-ttu-id="27b35-110">Valor</span><span class="sxs-lookup"><span data-stu-id="27b35-110">Value</span></span>|<span data-ttu-id="27b35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="27b35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27b35-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="27b35-112">unknown</span></span>|<span data-ttu-id="27b35-113">,0</span><span class="sxs-lookup"><span data-stu-id="27b35-113">0</span></span>|<span data-ttu-id="27b35-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="27b35-114">Unknown result.</span></span>|
|<span data-ttu-id="27b35-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="27b35-115">success</span></span>|<span data-ttu-id="27b35-116">1</span><span class="sxs-lookup"><span data-stu-id="27b35-116">1</span></span>|<span data-ttu-id="27b35-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="27b35-117">Script is run successfully.</span></span>|
|<span data-ttu-id="27b35-118">fail</span><span class="sxs-lookup"><span data-stu-id="27b35-118">fail</span></span>|<span data-ttu-id="27b35-119">duas</span><span class="sxs-lookup"><span data-stu-id="27b35-119">2</span></span>|<span data-ttu-id="27b35-120">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="27b35-120">Script failed to run.</span></span>|
|<span data-ttu-id="27b35-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="27b35-121">scriptError</span></span>|<span data-ttu-id="27b35-122">3D</span><span class="sxs-lookup"><span data-stu-id="27b35-122">3</span></span>|<span data-ttu-id="27b35-123">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="27b35-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="27b35-124">função</span><span class="sxs-lookup"><span data-stu-id="27b35-124">pending</span></span>|<span data-ttu-id="27b35-125">4 </span><span class="sxs-lookup"><span data-stu-id="27b35-125">4</span></span>|<span data-ttu-id="27b35-126">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="27b35-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="27b35-127">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="27b35-127">notApplicable</span></span>|<span data-ttu-id="27b35-128">5 </span><span class="sxs-lookup"><span data-stu-id="27b35-128">5</span></span>|<span data-ttu-id="27b35-129">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27b35-129">Script is not applicable for this device.</span></span>|





