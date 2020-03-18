---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f4c1605734afef3caefc4b51e2c8a826d2f2cd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767817"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="26e82-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="26e82-103">runState enum type</span></span>

> <span data-ttu-id="26e82-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26e82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26e82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e82-106">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26e82-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="26e82-107">Membros</span><span class="sxs-lookup"><span data-stu-id="26e82-107">Members</span></span>
|<span data-ttu-id="26e82-108">Membro</span><span class="sxs-lookup"><span data-stu-id="26e82-108">Member</span></span>|<span data-ttu-id="26e82-109">Valor</span><span class="sxs-lookup"><span data-stu-id="26e82-109">Value</span></span>|<span data-ttu-id="26e82-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e82-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="26e82-111">unknown</span></span>|<span data-ttu-id="26e82-112">,0</span><span class="sxs-lookup"><span data-stu-id="26e82-112">0</span></span>|<span data-ttu-id="26e82-113">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="26e82-113">Unknown result.</span></span>|
|<span data-ttu-id="26e82-114">sucesso</span><span class="sxs-lookup"><span data-stu-id="26e82-114">success</span></span>|<span data-ttu-id="26e82-115">1</span><span class="sxs-lookup"><span data-stu-id="26e82-115">1</span></span>|<span data-ttu-id="26e82-116">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="26e82-116">Script is run successfully.</span></span>|
|<span data-ttu-id="26e82-117">fail</span><span class="sxs-lookup"><span data-stu-id="26e82-117">fail</span></span>|<span data-ttu-id="26e82-118">duas</span><span class="sxs-lookup"><span data-stu-id="26e82-118">2</span></span>|<span data-ttu-id="26e82-119">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="26e82-119">Script failed to run.</span></span>|
|<span data-ttu-id="26e82-120">scriptError</span><span class="sxs-lookup"><span data-stu-id="26e82-120">scriptError</span></span>|<span data-ttu-id="26e82-121">3D</span><span class="sxs-lookup"><span data-stu-id="26e82-121">3</span></span>|<span data-ttu-id="26e82-122">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="26e82-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="26e82-123">função</span><span class="sxs-lookup"><span data-stu-id="26e82-123">pending</span></span>|<span data-ttu-id="26e82-124">4 </span><span class="sxs-lookup"><span data-stu-id="26e82-124">4</span></span>|<span data-ttu-id="26e82-125">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="26e82-125">Script is pending to execute.</span></span>|
|<span data-ttu-id="26e82-126">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="26e82-126">notApplicable</span></span>|<span data-ttu-id="26e82-127">5 </span><span class="sxs-lookup"><span data-stu-id="26e82-127">5</span></span>|<span data-ttu-id="26e82-128">O script não se aplica a este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26e82-128">Script is not applicable for this device.</span></span>|



