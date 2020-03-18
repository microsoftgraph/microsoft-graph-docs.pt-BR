---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 415c3b0df84c6b15a0185876280b82c7e8ed3d20
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777380"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="e6a3d-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="e6a3d-103">vppTokenState enum type</span></span>

> <span data-ttu-id="e6a3d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6a3d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6a3d-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="e6a3d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e6a3d-107">Members</span></span>
|<span data-ttu-id="e6a3d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e6a3d-108">Member</span></span>|<span data-ttu-id="e6a3d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e6a3d-109">Value</span></span>|<span data-ttu-id="e6a3d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a3d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6a3d-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e6a3d-111">unknown</span></span>|<span data-ttu-id="e6a3d-112">,0</span><span class="sxs-lookup"><span data-stu-id="e6a3d-112">0</span></span>|<span data-ttu-id="e6a3d-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-113">Default state.</span></span>|
|<span data-ttu-id="e6a3d-114">inválido</span><span class="sxs-lookup"><span data-stu-id="e6a3d-114">valid</span></span>|<span data-ttu-id="e6a3d-115">1</span><span class="sxs-lookup"><span data-stu-id="e6a3d-115">1</span></span>|<span data-ttu-id="e6a3d-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-116">Token is valid.</span></span>|
|<span data-ttu-id="e6a3d-117">venceu</span><span class="sxs-lookup"><span data-stu-id="e6a3d-117">expired</span></span>|<span data-ttu-id="e6a3d-118">duas</span><span class="sxs-lookup"><span data-stu-id="e6a3d-118">2</span></span>|<span data-ttu-id="e6a3d-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-119">Token is expired.</span></span>|
|<span data-ttu-id="e6a3d-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="e6a3d-120">invalid</span></span>|<span data-ttu-id="e6a3d-121">3D</span><span class="sxs-lookup"><span data-stu-id="e6a3d-121">3</span></span>|<span data-ttu-id="e6a3d-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-122">Token is invalid.</span></span>|
|<span data-ttu-id="e6a3d-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="e6a3d-123">assignedToExternalMDM</span></span>|<span data-ttu-id="e6a3d-124">4 </span><span class="sxs-lookup"><span data-stu-id="e6a3d-124">4</span></span>|<span data-ttu-id="e6a3d-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="e6a3d-125">Token is managed by another MDM Service.</span></span>|



