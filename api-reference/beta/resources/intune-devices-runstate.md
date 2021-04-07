---
title: Tipo de número runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612114"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="394f8-103">Tipo de número runState</span><span class="sxs-lookup"><span data-stu-id="394f8-103">runState enum type</span></span>

<span data-ttu-id="394f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="394f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="394f8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="394f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="394f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="394f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="394f8-107">Indica o tipo de status de execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="394f8-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="394f8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="394f8-108">Members</span></span>
|<span data-ttu-id="394f8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="394f8-109">Member</span></span>|<span data-ttu-id="394f8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="394f8-110">Value</span></span>|<span data-ttu-id="394f8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="394f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="394f8-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="394f8-112">unknown</span></span>|<span data-ttu-id="394f8-113">0</span><span class="sxs-lookup"><span data-stu-id="394f8-113">0</span></span>|<span data-ttu-id="394f8-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="394f8-114">Unknown result.</span></span>|
|<span data-ttu-id="394f8-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="394f8-115">success</span></span>|<span data-ttu-id="394f8-116">1</span><span class="sxs-lookup"><span data-stu-id="394f8-116">1</span></span>|<span data-ttu-id="394f8-117">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="394f8-117">Script is run successfully.</span></span>|
|<span data-ttu-id="394f8-118">fail</span><span class="sxs-lookup"><span data-stu-id="394f8-118">fail</span></span>|<span data-ttu-id="394f8-119">2</span><span class="sxs-lookup"><span data-stu-id="394f8-119">2</span></span>|<span data-ttu-id="394f8-120">Falha ao executar o script.</span><span class="sxs-lookup"><span data-stu-id="394f8-120">Script failed to run.</span></span>|
|<span data-ttu-id="394f8-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="394f8-121">scriptError</span></span>|<span data-ttu-id="394f8-122">3</span><span class="sxs-lookup"><span data-stu-id="394f8-122">3</span></span>|<span data-ttu-id="394f8-123">Erro de acertos de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="394f8-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="394f8-124">pendente</span><span class="sxs-lookup"><span data-stu-id="394f8-124">pending</span></span>|<span data-ttu-id="394f8-125">4 </span><span class="sxs-lookup"><span data-stu-id="394f8-125">4</span></span>|<span data-ttu-id="394f8-126">O script está pendente para ser executado.</span><span class="sxs-lookup"><span data-stu-id="394f8-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="394f8-127">notApplicable</span><span class="sxs-lookup"><span data-stu-id="394f8-127">notApplicable</span></span>|<span data-ttu-id="394f8-128">5 </span><span class="sxs-lookup"><span data-stu-id="394f8-128">5</span></span>|<span data-ttu-id="394f8-129">Script não é aplicável para este dispositivo.</span><span class="sxs-lookup"><span data-stu-id="394f8-129">Script is not applicable for this device.</span></span>|




