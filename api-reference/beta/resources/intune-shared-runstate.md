---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255816"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="45d8b-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="45d8b-103">runState enum type</span></span>

<span data-ttu-id="45d8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45d8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d8b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45d8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45d8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d8b-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45d8b-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="45d8b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="45d8b-108">Members</span></span>
|<span data-ttu-id="45d8b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="45d8b-109">Member</span></span>|<span data-ttu-id="45d8b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="45d8b-110">Value</span></span>|<span data-ttu-id="45d8b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45d8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d8b-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="45d8b-112">unknown</span></span>|<span data-ttu-id="45d8b-113">,0</span><span class="sxs-lookup"><span data-stu-id="45d8b-113">0</span></span>|<span data-ttu-id="45d8b-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="45d8b-114">Unknown result.</span></span>|
|<span data-ttu-id="45d8b-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="45d8b-115">success</span></span>|<span data-ttu-id="45d8b-116">1</span><span class="sxs-lookup"><span data-stu-id="45d8b-116">1</span></span>|<span data-ttu-id="45d8b-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="45d8b-117">Script is run successfully.</span></span>|
|<span data-ttu-id="45d8b-118">fail</span><span class="sxs-lookup"><span data-stu-id="45d8b-118">fail</span></span>|<span data-ttu-id="45d8b-119">duas</span><span class="sxs-lookup"><span data-stu-id="45d8b-119">2</span></span>|<span data-ttu-id="45d8b-120">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="45d8b-120">Script failed to run.</span></span>|
|<span data-ttu-id="45d8b-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="45d8b-121">scriptError</span></span>|<span data-ttu-id="45d8b-122">3D</span><span class="sxs-lookup"><span data-stu-id="45d8b-122">3</span></span>|<span data-ttu-id="45d8b-123">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="45d8b-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="45d8b-124">função</span><span class="sxs-lookup"><span data-stu-id="45d8b-124">pending</span></span>|<span data-ttu-id="45d8b-125">4 </span><span class="sxs-lookup"><span data-stu-id="45d8b-125">4</span></span>|<span data-ttu-id="45d8b-126">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="45d8b-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="45d8b-127">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="45d8b-127">notApplicable</span></span>|<span data-ttu-id="45d8b-128">5 </span><span class="sxs-lookup"><span data-stu-id="45d8b-128">5</span></span>|<span data-ttu-id="45d8b-129">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45d8b-129">Script is not applicable for this device.</span></span>|




