---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: faef244a196ae99a9ba82f4c5396db22b79be8b5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958512"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="cdc93-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="cdc93-103">vppTokenState enum type</span></span>

> <span data-ttu-id="cdc93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdc93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdc93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc93-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="cdc93-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="cdc93-107">Membros</span><span class="sxs-lookup"><span data-stu-id="cdc93-107">Members</span></span>
|<span data-ttu-id="cdc93-108">Membro</span><span class="sxs-lookup"><span data-stu-id="cdc93-108">Member</span></span>|<span data-ttu-id="cdc93-109">Valor</span><span class="sxs-lookup"><span data-stu-id="cdc93-109">Value</span></span>|<span data-ttu-id="cdc93-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc93-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="cdc93-111">unknown</span></span>|<span data-ttu-id="cdc93-112">,0</span><span class="sxs-lookup"><span data-stu-id="cdc93-112">0</span></span>|<span data-ttu-id="cdc93-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="cdc93-113">Default state.</span></span>|
|<span data-ttu-id="cdc93-114">inválido</span><span class="sxs-lookup"><span data-stu-id="cdc93-114">valid</span></span>|<span data-ttu-id="cdc93-115">1</span><span class="sxs-lookup"><span data-stu-id="cdc93-115">1</span></span>|<span data-ttu-id="cdc93-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="cdc93-116">Token is valid.</span></span>|
|<span data-ttu-id="cdc93-117">venceu</span><span class="sxs-lookup"><span data-stu-id="cdc93-117">expired</span></span>|<span data-ttu-id="cdc93-118">duas</span><span class="sxs-lookup"><span data-stu-id="cdc93-118">2</span></span>|<span data-ttu-id="cdc93-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="cdc93-119">Token is expired.</span></span>|
|<span data-ttu-id="cdc93-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="cdc93-120">invalid</span></span>|<span data-ttu-id="cdc93-121">3D</span><span class="sxs-lookup"><span data-stu-id="cdc93-121">3</span></span>|<span data-ttu-id="cdc93-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="cdc93-122">Token is invalid.</span></span>|
|<span data-ttu-id="cdc93-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="cdc93-123">assignedToExternalMDM</span></span>|<span data-ttu-id="cdc93-124">quatro</span><span class="sxs-lookup"><span data-stu-id="cdc93-124">4</span></span>|<span data-ttu-id="cdc93-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="cdc93-125">Token is managed by another MDM Service.</span></span>|





