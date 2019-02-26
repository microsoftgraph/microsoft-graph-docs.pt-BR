---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254930"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="ec505-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ec505-103">vppTokenState enum type</span></span>

> <span data-ttu-id="ec505-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec505-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec505-105">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec505-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="ec505-106">Membros</span><span class="sxs-lookup"><span data-stu-id="ec505-106">Members</span></span>
|<span data-ttu-id="ec505-107">Membro</span><span class="sxs-lookup"><span data-stu-id="ec505-107">Member</span></span>|<span data-ttu-id="ec505-108">Valor</span><span class="sxs-lookup"><span data-stu-id="ec505-108">Value</span></span>|<span data-ttu-id="ec505-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec505-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec505-110">unknown</span><span class="sxs-lookup"><span data-stu-id="ec505-110">unknown</span></span>|<span data-ttu-id="ec505-111">,0</span><span class="sxs-lookup"><span data-stu-id="ec505-111">0</span></span>|<span data-ttu-id="ec505-112">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="ec505-112">Default state.</span></span>|
|<span data-ttu-id="ec505-113">inválido</span><span class="sxs-lookup"><span data-stu-id="ec505-113">valid</span></span>|<span data-ttu-id="ec505-114">1</span><span class="sxs-lookup"><span data-stu-id="ec505-114">1</span></span>|<span data-ttu-id="ec505-115">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="ec505-115">Token is valid.</span></span>|
|<span data-ttu-id="ec505-116">venceu</span><span class="sxs-lookup"><span data-stu-id="ec505-116">expired</span></span>|<span data-ttu-id="ec505-117">duas</span><span class="sxs-lookup"><span data-stu-id="ec505-117">2</span></span>|<span data-ttu-id="ec505-118">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="ec505-118">Token is expired.</span></span>|
|<span data-ttu-id="ec505-119">Inválido</span><span class="sxs-lookup"><span data-stu-id="ec505-119">invalid</span></span>|<span data-ttu-id="ec505-120">3D</span><span class="sxs-lookup"><span data-stu-id="ec505-120">3</span></span>|<span data-ttu-id="ec505-121">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="ec505-121">Token is invalid.</span></span>|
|<span data-ttu-id="ec505-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="ec505-122">assignedToExternalMDM</span></span>|<span data-ttu-id="ec505-123">quatro</span><span class="sxs-lookup"><span data-stu-id="ec505-123">4</span></span>|<span data-ttu-id="ec505-124">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="ec505-124">Token is managed by another MDM Service.</span></span>|



