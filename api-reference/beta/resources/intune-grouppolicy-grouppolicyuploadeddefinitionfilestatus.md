---
title: tipo de enumeração groupPolicyUploadedDefinitionFileStatus
description: Tipo de política de grupo carregou o status do arquivo de definição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6afafd9f6e35d248b69c3b7ddbb24c20e60d0eeb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298082"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="6a7c4-103">tipo de enumeração groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="6a7c4-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="6a7c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a7c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a7c4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a7c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7c4-107">Tipo de política de grupo carregou o status do arquivo de definição.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="6a7c4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6a7c4-108">Members</span></span>
|<span data-ttu-id="6a7c4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6a7c4-109">Member</span></span>|<span data-ttu-id="6a7c4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6a7c4-110">Value</span></span>|<span data-ttu-id="6a7c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a7c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7c4-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="6a7c4-112">none</span></span>|<span data-ttu-id="6a7c4-113">,0</span><span class="sxs-lookup"><span data-stu-id="6a7c4-113">0</span></span>|<span data-ttu-id="6a7c4-114">Política de grupo carregou o arquivo de definição inválido status de carregamento.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="6a7c4-115">uploadInProgress</span><span class="sxs-lookup"><span data-stu-id="6a7c4-115">uploadInProgress</span></span>|<span data-ttu-id="6a7c4-116">1</span><span class="sxs-lookup"><span data-stu-id="6a7c4-116">1</span></span>|<span data-ttu-id="6a7c4-117">Carregamento de arquivo de definição carregado da política de grupo em andamento.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="6a7c4-118">disponível</span><span class="sxs-lookup"><span data-stu-id="6a7c4-118">available</span></span>|<span data-ttu-id="6a7c4-119">duas</span><span class="sxs-lookup"><span data-stu-id="6a7c4-119">2</span></span>|<span data-ttu-id="6a7c4-120">Arquivo de definição de política de grupo carregado disponível.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="6a7c4-121">atribuí</span><span class="sxs-lookup"><span data-stu-id="6a7c4-121">assigned</span></span>|<span data-ttu-id="6a7c4-122">3D</span><span class="sxs-lookup"><span data-stu-id="6a7c4-122">3</span></span>|<span data-ttu-id="6a7c4-123">Política de grupo carregou o arquivo de definição atribuído à política.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="6a7c4-124">removalInProgress</span><span class="sxs-lookup"><span data-stu-id="6a7c4-124">removalInProgress</span></span>|<span data-ttu-id="6a7c4-125">4 </span><span class="sxs-lookup"><span data-stu-id="6a7c4-125">4</span></span>|<span data-ttu-id="6a7c4-126">Política de grupo carregou a remoção de arquivo de definição em andamento.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="6a7c4-127">uploadFailed</span><span class="sxs-lookup"><span data-stu-id="6a7c4-127">uploadFailed</span></span>|<span data-ttu-id="6a7c4-128">5 </span><span class="sxs-lookup"><span data-stu-id="6a7c4-128">5</span></span>|<span data-ttu-id="6a7c4-129">Falha no carregamento de arquivo de definição de política de grupo carregado.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="6a7c4-130">removalFailed</span><span class="sxs-lookup"><span data-stu-id="6a7c4-130">removalFailed</span></span>|<span data-ttu-id="6a7c4-131">6 </span><span class="sxs-lookup"><span data-stu-id="6a7c4-131">6</span></span>|<span data-ttu-id="6a7c4-132">A política de grupo carregou a remoção de arquivo de definição falhou.</span><span class="sxs-lookup"><span data-stu-id="6a7c4-132">Group Policy uploaded definition file removal failed.</span></span>|




