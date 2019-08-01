---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c1effcc94eb7ed0929902c935c848e4610c1971b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037224"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="55753-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="55753-103">vppTokenState enum type</span></span>

> <span data-ttu-id="55753-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55753-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55753-105">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="55753-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="55753-106">Membros</span><span class="sxs-lookup"><span data-stu-id="55753-106">Members</span></span>
|<span data-ttu-id="55753-107">Membro</span><span class="sxs-lookup"><span data-stu-id="55753-107">Member</span></span>|<span data-ttu-id="55753-108">Valor</span><span class="sxs-lookup"><span data-stu-id="55753-108">Value</span></span>|<span data-ttu-id="55753-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55753-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55753-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="55753-110">unknown</span></span>|<span data-ttu-id="55753-111">,0</span><span class="sxs-lookup"><span data-stu-id="55753-111">0</span></span>|<span data-ttu-id="55753-112">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="55753-112">Default state.</span></span>|
|<span data-ttu-id="55753-113">inválido</span><span class="sxs-lookup"><span data-stu-id="55753-113">valid</span></span>|<span data-ttu-id="55753-114">1</span><span class="sxs-lookup"><span data-stu-id="55753-114">1</span></span>|<span data-ttu-id="55753-115">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="55753-115">Token is valid.</span></span>|
|<span data-ttu-id="55753-116">venceu</span><span class="sxs-lookup"><span data-stu-id="55753-116">expired</span></span>|<span data-ttu-id="55753-117">duas</span><span class="sxs-lookup"><span data-stu-id="55753-117">2</span></span>|<span data-ttu-id="55753-118">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="55753-118">Token is expired.</span></span>|
|<span data-ttu-id="55753-119">Inválido</span><span class="sxs-lookup"><span data-stu-id="55753-119">invalid</span></span>|<span data-ttu-id="55753-120">3D</span><span class="sxs-lookup"><span data-stu-id="55753-120">3</span></span>|<span data-ttu-id="55753-121">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="55753-121">Token is invalid.</span></span>|
|<span data-ttu-id="55753-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="55753-122">assignedToExternalMDM</span></span>|<span data-ttu-id="55753-123">quatro</span><span class="sxs-lookup"><span data-stu-id="55753-123">4</span></span>|<span data-ttu-id="55753-124">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="55753-124">Token is managed by another MDM Service.</span></span>|



