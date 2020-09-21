---
title: tipo de enumeração groupPolicyUploadedDefinitionFileStatus
description: Tipo de política de grupo carregou o status do arquivo de definição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70430e74d332baf0b1c81a41d2098883688464ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030609"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="e4777-103">tipo de enumeração groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="e4777-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="e4777-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4777-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4777-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4777-107">Tipo de política de grupo carregou o status do arquivo de definição.</span><span class="sxs-lookup"><span data-stu-id="e4777-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="e4777-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e4777-108">Members</span></span>
|<span data-ttu-id="e4777-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e4777-109">Member</span></span>|<span data-ttu-id="e4777-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e4777-110">Value</span></span>|<span data-ttu-id="e4777-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4777-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4777-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e4777-112">none</span></span>|<span data-ttu-id="e4777-113">,0</span><span class="sxs-lookup"><span data-stu-id="e4777-113">0</span></span>|<span data-ttu-id="e4777-114">Política de grupo carregou o arquivo de definição inválido status de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e4777-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="e4777-115">uploadInProgress</span><span class="sxs-lookup"><span data-stu-id="e4777-115">uploadInProgress</span></span>|<span data-ttu-id="e4777-116">1 </span><span class="sxs-lookup"><span data-stu-id="e4777-116">1</span></span>|<span data-ttu-id="e4777-117">Carregamento de arquivo de definição carregado da política de grupo em andamento.</span><span class="sxs-lookup"><span data-stu-id="e4777-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="e4777-118">disponível</span><span class="sxs-lookup"><span data-stu-id="e4777-118">available</span></span>|<span data-ttu-id="e4777-119">2 </span><span class="sxs-lookup"><span data-stu-id="e4777-119">2</span></span>|<span data-ttu-id="e4777-120">Arquivo de definição de política de grupo carregado disponível.</span><span class="sxs-lookup"><span data-stu-id="e4777-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="e4777-121">atribuí</span><span class="sxs-lookup"><span data-stu-id="e4777-121">assigned</span></span>|<span data-ttu-id="e4777-122">3 </span><span class="sxs-lookup"><span data-stu-id="e4777-122">3</span></span>|<span data-ttu-id="e4777-123">Política de grupo carregou o arquivo de definição atribuído à política.</span><span class="sxs-lookup"><span data-stu-id="e4777-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="e4777-124">removalInProgress</span><span class="sxs-lookup"><span data-stu-id="e4777-124">removalInProgress</span></span>|<span data-ttu-id="e4777-125">4 </span><span class="sxs-lookup"><span data-stu-id="e4777-125">4</span></span>|<span data-ttu-id="e4777-126">Política de grupo carregou a remoção de arquivo de definição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e4777-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="e4777-127">uploadFailed</span><span class="sxs-lookup"><span data-stu-id="e4777-127">uploadFailed</span></span>|<span data-ttu-id="e4777-128">5 </span><span class="sxs-lookup"><span data-stu-id="e4777-128">5</span></span>|<span data-ttu-id="e4777-129">Falha no carregamento de arquivo de definição de política de grupo carregado.</span><span class="sxs-lookup"><span data-stu-id="e4777-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="e4777-130">removalFailed</span><span class="sxs-lookup"><span data-stu-id="e4777-130">removalFailed</span></span>|<span data-ttu-id="e4777-131">6 </span><span class="sxs-lookup"><span data-stu-id="e4777-131">6</span></span>|<span data-ttu-id="e4777-132">A política de grupo carregou a remoção de arquivo de definição falhou.</span><span class="sxs-lookup"><span data-stu-id="e4777-132">Group Policy uploaded definition file removal failed.</span></span>|






