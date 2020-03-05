---
title: tipo de enumeração deviceManagementReportStatus
description: Status possíveis associados a um relatório gerado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e549e2ca96e272930c13aa07f0e35e2143e96c2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527510"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="1b176-103">tipo de enumeração deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="1b176-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="1b176-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1b176-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b176-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b176-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b176-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b176-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b176-107">Status possíveis associados a um relatório gerado</span><span class="sxs-lookup"><span data-stu-id="1b176-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="1b176-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1b176-108">Members</span></span>
|<span data-ttu-id="1b176-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1b176-109">Member</span></span>|<span data-ttu-id="1b176-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1b176-110">Value</span></span>|<span data-ttu-id="1b176-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b176-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b176-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="1b176-112">unknown</span></span>|<span data-ttu-id="1b176-113">,0</span><span class="sxs-lookup"><span data-stu-id="1b176-113">0</span></span>|<span data-ttu-id="1b176-114">O status da geração de relatórios é desconhecido</span><span class="sxs-lookup"><span data-stu-id="1b176-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="1b176-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="1b176-115">notStarted</span></span>|<span data-ttu-id="1b176-116">1 </span><span class="sxs-lookup"><span data-stu-id="1b176-116">1</span></span>|<span data-ttu-id="1b176-117">A geração de relatório não foi iniciada</span><span class="sxs-lookup"><span data-stu-id="1b176-117">Report generation has not started</span></span>|
|<span data-ttu-id="1b176-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="1b176-118">inProgress</span></span>|<span data-ttu-id="1b176-119">2 </span><span class="sxs-lookup"><span data-stu-id="1b176-119">2</span></span>|<span data-ttu-id="1b176-120">Geração de relatório em andamento</span><span class="sxs-lookup"><span data-stu-id="1b176-120">Report generation is in progress</span></span>|
|<span data-ttu-id="1b176-121">Completed</span><span class="sxs-lookup"><span data-stu-id="1b176-121">completed</span></span>|<span data-ttu-id="1b176-122">3 </span><span class="sxs-lookup"><span data-stu-id="1b176-122">3</span></span>|<span data-ttu-id="1b176-123">Geração de relatório concluída</span><span class="sxs-lookup"><span data-stu-id="1b176-123">Report generation is completed</span></span>|
|<span data-ttu-id="1b176-124">falhou</span><span class="sxs-lookup"><span data-stu-id="1b176-124">failed</span></span>|<span data-ttu-id="1b176-125">4 </span><span class="sxs-lookup"><span data-stu-id="1b176-125">4</span></span>|<span data-ttu-id="1b176-126">A geração de relatórios falhou</span><span class="sxs-lookup"><span data-stu-id="1b176-126">Report generation has failed</span></span>|



