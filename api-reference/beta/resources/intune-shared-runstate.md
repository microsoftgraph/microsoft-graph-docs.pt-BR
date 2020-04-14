---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 37905590f5ca61db53f98ff047ef699549f269ae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473505"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="e3661-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="e3661-103">runState enum type</span></span>

<span data-ttu-id="e3661-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3661-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3661-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3661-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3661-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3661-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3661-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e3661-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="e3661-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e3661-108">Members</span></span>
|<span data-ttu-id="e3661-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e3661-109">Member</span></span>|<span data-ttu-id="e3661-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e3661-110">Value</span></span>|<span data-ttu-id="e3661-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3661-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3661-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e3661-112">unknown</span></span>|<span data-ttu-id="e3661-113">,0</span><span class="sxs-lookup"><span data-stu-id="e3661-113">0</span></span>|<span data-ttu-id="e3661-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e3661-114">Unknown result.</span></span>|
|<span data-ttu-id="e3661-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="e3661-115">success</span></span>|<span data-ttu-id="e3661-116">1</span><span class="sxs-lookup"><span data-stu-id="e3661-116">1</span></span>|<span data-ttu-id="e3661-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="e3661-117">Script is run successfully.</span></span>|
|<span data-ttu-id="e3661-118">fail</span><span class="sxs-lookup"><span data-stu-id="e3661-118">fail</span></span>|<span data-ttu-id="e3661-119">duas</span><span class="sxs-lookup"><span data-stu-id="e3661-119">2</span></span>|<span data-ttu-id="e3661-120">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="e3661-120">Script failed to run.</span></span>|
|<span data-ttu-id="e3661-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="e3661-121">scriptError</span></span>|<span data-ttu-id="e3661-122">3D</span><span class="sxs-lookup"><span data-stu-id="e3661-122">3</span></span>|<span data-ttu-id="e3661-123">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="e3661-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="e3661-124">função</span><span class="sxs-lookup"><span data-stu-id="e3661-124">pending</span></span>|<span data-ttu-id="e3661-125">4 </span><span class="sxs-lookup"><span data-stu-id="e3661-125">4</span></span>|<span data-ttu-id="e3661-126">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="e3661-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="e3661-127">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="e3661-127">notApplicable</span></span>|<span data-ttu-id="e3661-128">5 </span><span class="sxs-lookup"><span data-stu-id="e3661-128">5</span></span>|<span data-ttu-id="e3661-129">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e3661-129">Script is not applicable for this device.</span></span>|



