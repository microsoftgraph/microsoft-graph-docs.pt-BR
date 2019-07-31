---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d9ae2b3bfb45ff33c5f0a39d746350212db3027c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010634"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="1f8c8-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="1f8c8-103">vppTokenState enum type</span></span>

> <span data-ttu-id="1f8c8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f8c8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f8c8-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="1f8c8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1f8c8-107">Members</span></span>
|<span data-ttu-id="1f8c8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1f8c8-108">Member</span></span>|<span data-ttu-id="1f8c8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1f8c8-109">Value</span></span>|<span data-ttu-id="1f8c8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f8c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f8c8-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="1f8c8-111">unknown</span></span>|<span data-ttu-id="1f8c8-112">,0</span><span class="sxs-lookup"><span data-stu-id="1f8c8-112">0</span></span>|<span data-ttu-id="1f8c8-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-113">Default state.</span></span>|
|<span data-ttu-id="1f8c8-114">inválido</span><span class="sxs-lookup"><span data-stu-id="1f8c8-114">valid</span></span>|<span data-ttu-id="1f8c8-115">1</span><span class="sxs-lookup"><span data-stu-id="1f8c8-115">1</span></span>|<span data-ttu-id="1f8c8-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-116">Token is valid.</span></span>|
|<span data-ttu-id="1f8c8-117">venceu</span><span class="sxs-lookup"><span data-stu-id="1f8c8-117">expired</span></span>|<span data-ttu-id="1f8c8-118">duas</span><span class="sxs-lookup"><span data-stu-id="1f8c8-118">2</span></span>|<span data-ttu-id="1f8c8-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-119">Token is expired.</span></span>|
|<span data-ttu-id="1f8c8-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="1f8c8-120">invalid</span></span>|<span data-ttu-id="1f8c8-121">3D</span><span class="sxs-lookup"><span data-stu-id="1f8c8-121">3</span></span>|<span data-ttu-id="1f8c8-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-122">Token is invalid.</span></span>|
|<span data-ttu-id="1f8c8-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="1f8c8-123">assignedToExternalMDM</span></span>|<span data-ttu-id="1f8c8-124">quatro</span><span class="sxs-lookup"><span data-stu-id="1f8c8-124">4</span></span>|<span data-ttu-id="1f8c8-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="1f8c8-125">Token is managed by another MDM Service.</span></span>|





