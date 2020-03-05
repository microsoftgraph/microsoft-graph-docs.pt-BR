---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fef95d2d5744d0cdc6b92328b15a44f8b21c6cb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523545"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="93b03-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="93b03-103">runState enum type</span></span>

<span data-ttu-id="93b03-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="93b03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93b03-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93b03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93b03-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93b03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93b03-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93b03-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="93b03-108">Membros</span><span class="sxs-lookup"><span data-stu-id="93b03-108">Members</span></span>
|<span data-ttu-id="93b03-109">Membro</span><span class="sxs-lookup"><span data-stu-id="93b03-109">Member</span></span>|<span data-ttu-id="93b03-110">Valor</span><span class="sxs-lookup"><span data-stu-id="93b03-110">Value</span></span>|<span data-ttu-id="93b03-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93b03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93b03-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="93b03-112">unknown</span></span>|<span data-ttu-id="93b03-113">,0</span><span class="sxs-lookup"><span data-stu-id="93b03-113">0</span></span>|<span data-ttu-id="93b03-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="93b03-114">Unknown result.</span></span>|
|<span data-ttu-id="93b03-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="93b03-115">success</span></span>|<span data-ttu-id="93b03-116">1 </span><span class="sxs-lookup"><span data-stu-id="93b03-116">1</span></span>|<span data-ttu-id="93b03-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="93b03-117">Script is run successfully.</span></span>|
|<span data-ttu-id="93b03-118">fail</span><span class="sxs-lookup"><span data-stu-id="93b03-118">fail</span></span>|<span data-ttu-id="93b03-119">2 </span><span class="sxs-lookup"><span data-stu-id="93b03-119">2</span></span>|<span data-ttu-id="93b03-120">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="93b03-120">Script failed to run.</span></span>|
|<span data-ttu-id="93b03-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="93b03-121">scriptError</span></span>|<span data-ttu-id="93b03-122">3 </span><span class="sxs-lookup"><span data-stu-id="93b03-122">3</span></span>|<span data-ttu-id="93b03-123">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="93b03-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="93b03-124">função</span><span class="sxs-lookup"><span data-stu-id="93b03-124">pending</span></span>|<span data-ttu-id="93b03-125">4 </span><span class="sxs-lookup"><span data-stu-id="93b03-125">4</span></span>|<span data-ttu-id="93b03-126">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="93b03-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="93b03-127">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="93b03-127">notApplicable</span></span>|<span data-ttu-id="93b03-128">5 </span><span class="sxs-lookup"><span data-stu-id="93b03-128">5</span></span>|<span data-ttu-id="93b03-129">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93b03-129">Script is not applicable for this device.</span></span>|



