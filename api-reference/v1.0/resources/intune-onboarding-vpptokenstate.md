---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 52b184490f4653898383deeda6996e353964d9b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441718"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="0a37d-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="0a37d-103">vppTokenState enum type</span></span>

<span data-ttu-id="0a37d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a37d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a37d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a37d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a37d-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0a37d-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="0a37d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0a37d-107">Members</span></span>
|<span data-ttu-id="0a37d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0a37d-108">Member</span></span>|<span data-ttu-id="0a37d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0a37d-109">Value</span></span>|<span data-ttu-id="0a37d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a37d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a37d-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="0a37d-111">unknown</span></span>|<span data-ttu-id="0a37d-112">,0</span><span class="sxs-lookup"><span data-stu-id="0a37d-112">0</span></span>|<span data-ttu-id="0a37d-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="0a37d-113">Default state.</span></span>|
|<span data-ttu-id="0a37d-114">inválido</span><span class="sxs-lookup"><span data-stu-id="0a37d-114">valid</span></span>|<span data-ttu-id="0a37d-115">1</span><span class="sxs-lookup"><span data-stu-id="0a37d-115">1</span></span>|<span data-ttu-id="0a37d-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="0a37d-116">Token is valid.</span></span>|
|<span data-ttu-id="0a37d-117">venceu</span><span class="sxs-lookup"><span data-stu-id="0a37d-117">expired</span></span>|<span data-ttu-id="0a37d-118">duas</span><span class="sxs-lookup"><span data-stu-id="0a37d-118">2</span></span>|<span data-ttu-id="0a37d-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="0a37d-119">Token is expired.</span></span>|
|<span data-ttu-id="0a37d-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="0a37d-120">invalid</span></span>|<span data-ttu-id="0a37d-121">3D</span><span class="sxs-lookup"><span data-stu-id="0a37d-121">3</span></span>|<span data-ttu-id="0a37d-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="0a37d-122">Token is invalid.</span></span>|
|<span data-ttu-id="0a37d-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="0a37d-123">assignedToExternalMDM</span></span>|<span data-ttu-id="0a37d-124">4 </span><span class="sxs-lookup"><span data-stu-id="0a37d-124">4</span></span>|<span data-ttu-id="0a37d-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="0a37d-125">Token is managed by another MDM Service.</span></span>|







