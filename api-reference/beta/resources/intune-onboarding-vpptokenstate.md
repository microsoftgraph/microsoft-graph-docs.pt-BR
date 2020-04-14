---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21979c33bc1dcc06b83f9169341aa67ca516f066
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446820"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="5e500-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="5e500-103">vppTokenState enum type</span></span>

<span data-ttu-id="5e500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e500-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e500-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e500-107">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5e500-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="5e500-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5e500-108">Members</span></span>
|<span data-ttu-id="5e500-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5e500-109">Member</span></span>|<span data-ttu-id="5e500-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5e500-110">Value</span></span>|<span data-ttu-id="5e500-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e500-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e500-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5e500-112">unknown</span></span>|<span data-ttu-id="5e500-113">,0</span><span class="sxs-lookup"><span data-stu-id="5e500-113">0</span></span>|<span data-ttu-id="5e500-114">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="5e500-114">Default state.</span></span>|
|<span data-ttu-id="5e500-115">inválido</span><span class="sxs-lookup"><span data-stu-id="5e500-115">valid</span></span>|<span data-ttu-id="5e500-116">1</span><span class="sxs-lookup"><span data-stu-id="5e500-116">1</span></span>|<span data-ttu-id="5e500-117">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="5e500-117">Token is valid.</span></span>|
|<span data-ttu-id="5e500-118">venceu</span><span class="sxs-lookup"><span data-stu-id="5e500-118">expired</span></span>|<span data-ttu-id="5e500-119">duas</span><span class="sxs-lookup"><span data-stu-id="5e500-119">2</span></span>|<span data-ttu-id="5e500-120">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="5e500-120">Token is expired.</span></span>|
|<span data-ttu-id="5e500-121">Inválido</span><span class="sxs-lookup"><span data-stu-id="5e500-121">invalid</span></span>|<span data-ttu-id="5e500-122">3D</span><span class="sxs-lookup"><span data-stu-id="5e500-122">3</span></span>|<span data-ttu-id="5e500-123">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="5e500-123">Token is invalid.</span></span>|
|<span data-ttu-id="5e500-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="5e500-124">assignedToExternalMDM</span></span>|<span data-ttu-id="5e500-125">4 </span><span class="sxs-lookup"><span data-stu-id="5e500-125">4</span></span>|<span data-ttu-id="5e500-126">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="5e500-126">Token is managed by another MDM Service.</span></span>|



