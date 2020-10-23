---
title: tipo de enumeração groupPolicyUploadedDefinitionFileStatus
description: Tipo de política de grupo carregou o status do arquivo de definição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9b9456b5eb4ec3486aebc877d42651d0496f117c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707700"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="e31ab-103">tipo de enumeração groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="e31ab-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="e31ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e31ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e31ab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e31ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e31ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e31ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e31ab-107">Tipo de política de grupo carregou o status do arquivo de definição.</span><span class="sxs-lookup"><span data-stu-id="e31ab-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="e31ab-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e31ab-108">Members</span></span>
|<span data-ttu-id="e31ab-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e31ab-109">Member</span></span>|<span data-ttu-id="e31ab-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e31ab-110">Value</span></span>|<span data-ttu-id="e31ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e31ab-112">none</span><span class="sxs-lookup"><span data-stu-id="e31ab-112">none</span></span>|<span data-ttu-id="e31ab-113">,0</span><span class="sxs-lookup"><span data-stu-id="e31ab-113">0</span></span>|<span data-ttu-id="e31ab-114">Política de grupo carregou o arquivo de definição inválido status de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e31ab-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="e31ab-115">uploadInProgress</span><span class="sxs-lookup"><span data-stu-id="e31ab-115">uploadInProgress</span></span>|<span data-ttu-id="e31ab-116">1</span><span class="sxs-lookup"><span data-stu-id="e31ab-116">1</span></span>|<span data-ttu-id="e31ab-117">Carregamento de arquivo de definição carregado da política de grupo em andamento.</span><span class="sxs-lookup"><span data-stu-id="e31ab-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="e31ab-118">disponível</span><span class="sxs-lookup"><span data-stu-id="e31ab-118">available</span></span>|<span data-ttu-id="e31ab-119">duas</span><span class="sxs-lookup"><span data-stu-id="e31ab-119">2</span></span>|<span data-ttu-id="e31ab-120">Arquivo de definição de política de grupo carregado disponível.</span><span class="sxs-lookup"><span data-stu-id="e31ab-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="e31ab-121">atribuí</span><span class="sxs-lookup"><span data-stu-id="e31ab-121">assigned</span></span>|<span data-ttu-id="e31ab-122">3D</span><span class="sxs-lookup"><span data-stu-id="e31ab-122">3</span></span>|<span data-ttu-id="e31ab-123">Política de grupo carregou o arquivo de definição atribuído à política.</span><span class="sxs-lookup"><span data-stu-id="e31ab-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="e31ab-124">removalInProgress</span><span class="sxs-lookup"><span data-stu-id="e31ab-124">removalInProgress</span></span>|<span data-ttu-id="e31ab-125">4 </span><span class="sxs-lookup"><span data-stu-id="e31ab-125">4</span></span>|<span data-ttu-id="e31ab-126">Política de grupo carregou a remoção de arquivo de definição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e31ab-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="e31ab-127">uploadFailed</span><span class="sxs-lookup"><span data-stu-id="e31ab-127">uploadFailed</span></span>|<span data-ttu-id="e31ab-128">5 </span><span class="sxs-lookup"><span data-stu-id="e31ab-128">5</span></span>|<span data-ttu-id="e31ab-129">Falha no carregamento de arquivo de definição de política de grupo carregado.</span><span class="sxs-lookup"><span data-stu-id="e31ab-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="e31ab-130">removalFailed</span><span class="sxs-lookup"><span data-stu-id="e31ab-130">removalFailed</span></span>|<span data-ttu-id="e31ab-131">6 </span><span class="sxs-lookup"><span data-stu-id="e31ab-131">6</span></span>|<span data-ttu-id="e31ab-132">A política de grupo carregou a remoção de arquivo de definição falhou.</span><span class="sxs-lookup"><span data-stu-id="e31ab-132">Group Policy uploaded definition file removal failed.</span></span>|





