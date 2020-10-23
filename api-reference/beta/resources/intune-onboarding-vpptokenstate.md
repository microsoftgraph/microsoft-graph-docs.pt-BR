---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 886dd49a1ab963141b19b450619423372295c052
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703605"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="6755d-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="6755d-103">vppTokenState enum type</span></span>

<span data-ttu-id="6755d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6755d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6755d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6755d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6755d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6755d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6755d-107">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6755d-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="6755d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6755d-108">Members</span></span>
|<span data-ttu-id="6755d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6755d-109">Member</span></span>|<span data-ttu-id="6755d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6755d-110">Value</span></span>|<span data-ttu-id="6755d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6755d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6755d-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6755d-112">unknown</span></span>|<span data-ttu-id="6755d-113">,0</span><span class="sxs-lookup"><span data-stu-id="6755d-113">0</span></span>|<span data-ttu-id="6755d-114">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="6755d-114">Default state.</span></span>|
|<span data-ttu-id="6755d-115">inválido</span><span class="sxs-lookup"><span data-stu-id="6755d-115">valid</span></span>|<span data-ttu-id="6755d-116">1</span><span class="sxs-lookup"><span data-stu-id="6755d-116">1</span></span>|<span data-ttu-id="6755d-117">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="6755d-117">Token is valid.</span></span>|
|<span data-ttu-id="6755d-118">venceu</span><span class="sxs-lookup"><span data-stu-id="6755d-118">expired</span></span>|<span data-ttu-id="6755d-119">duas</span><span class="sxs-lookup"><span data-stu-id="6755d-119">2</span></span>|<span data-ttu-id="6755d-120">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="6755d-120">Token is expired.</span></span>|
|<span data-ttu-id="6755d-121">Inválido</span><span class="sxs-lookup"><span data-stu-id="6755d-121">invalid</span></span>|<span data-ttu-id="6755d-122">3D</span><span class="sxs-lookup"><span data-stu-id="6755d-122">3</span></span>|<span data-ttu-id="6755d-123">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="6755d-123">Token is invalid.</span></span>|
|<span data-ttu-id="6755d-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="6755d-124">assignedToExternalMDM</span></span>|<span data-ttu-id="6755d-125">4 </span><span class="sxs-lookup"><span data-stu-id="6755d-125">4</span></span>|<span data-ttu-id="6755d-126">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="6755d-126">Token is managed by another MDM Service.</span></span>|
|<span data-ttu-id="6755d-127">duplicateLocationId</span><span class="sxs-lookup"><span data-stu-id="6755d-127">duplicateLocationId</span></span>|<span data-ttu-id="6755d-128">5 </span><span class="sxs-lookup"><span data-stu-id="6755d-128">5</span></span>|<span data-ttu-id="6755d-129">O token é associado ao mesmo local de outro token na conta.</span><span class="sxs-lookup"><span data-stu-id="6755d-129">Token is associated with the same location as another token on the account.</span></span>|





