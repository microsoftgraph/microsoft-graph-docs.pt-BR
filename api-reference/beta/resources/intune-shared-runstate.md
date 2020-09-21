---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36022987fb96671399523a5936c7799e97db33c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084041"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="35eec-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="35eec-103">runState enum type</span></span>

<span data-ttu-id="35eec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35eec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35eec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35eec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35eec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35eec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35eec-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35eec-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="35eec-108">Membros</span><span class="sxs-lookup"><span data-stu-id="35eec-108">Members</span></span>
|<span data-ttu-id="35eec-109">Membro</span><span class="sxs-lookup"><span data-stu-id="35eec-109">Member</span></span>|<span data-ttu-id="35eec-110">Valor</span><span class="sxs-lookup"><span data-stu-id="35eec-110">Value</span></span>|<span data-ttu-id="35eec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35eec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35eec-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="35eec-112">unknown</span></span>|<span data-ttu-id="35eec-113">,0</span><span class="sxs-lookup"><span data-stu-id="35eec-113">0</span></span>|<span data-ttu-id="35eec-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="35eec-114">Unknown result.</span></span>|
|<span data-ttu-id="35eec-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="35eec-115">success</span></span>|<span data-ttu-id="35eec-116">1 </span><span class="sxs-lookup"><span data-stu-id="35eec-116">1</span></span>|<span data-ttu-id="35eec-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="35eec-117">Script is run successfully.</span></span>|
|<span data-ttu-id="35eec-118">fail</span><span class="sxs-lookup"><span data-stu-id="35eec-118">fail</span></span>|<span data-ttu-id="35eec-119">2 </span><span class="sxs-lookup"><span data-stu-id="35eec-119">2</span></span>|<span data-ttu-id="35eec-120">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="35eec-120">Script failed to run.</span></span>|
|<span data-ttu-id="35eec-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="35eec-121">scriptError</span></span>|<span data-ttu-id="35eec-122">3D</span><span class="sxs-lookup"><span data-stu-id="35eec-122">3</span></span>|<span data-ttu-id="35eec-123">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="35eec-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="35eec-124">função</span><span class="sxs-lookup"><span data-stu-id="35eec-124">pending</span></span>|<span data-ttu-id="35eec-125">4 </span><span class="sxs-lookup"><span data-stu-id="35eec-125">4</span></span>|<span data-ttu-id="35eec-126">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="35eec-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="35eec-127">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="35eec-127">notApplicable</span></span>|<span data-ttu-id="35eec-128">5 </span><span class="sxs-lookup"><span data-stu-id="35eec-128">5</span></span>|<span data-ttu-id="35eec-129">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35eec-129">Script is not applicable for this device.</span></span>|






