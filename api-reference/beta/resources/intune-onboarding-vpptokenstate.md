---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3e78e5762c1d59d882973a44f69482fcb21998f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527684"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="f948c-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="f948c-103">vppTokenState enum type</span></span>

<span data-ttu-id="f948c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f948c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f948c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f948c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f948c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f948c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f948c-107">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f948c-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="f948c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f948c-108">Members</span></span>
|<span data-ttu-id="f948c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f948c-109">Member</span></span>|<span data-ttu-id="f948c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f948c-110">Value</span></span>|<span data-ttu-id="f948c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f948c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f948c-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f948c-112">unknown</span></span>|<span data-ttu-id="f948c-113">,0</span><span class="sxs-lookup"><span data-stu-id="f948c-113">0</span></span>|<span data-ttu-id="f948c-114">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="f948c-114">Default state.</span></span>|
|<span data-ttu-id="f948c-115">inválido</span><span class="sxs-lookup"><span data-stu-id="f948c-115">valid</span></span>|<span data-ttu-id="f948c-116">1 </span><span class="sxs-lookup"><span data-stu-id="f948c-116">1</span></span>|<span data-ttu-id="f948c-117">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="f948c-117">Token is valid.</span></span>|
|<span data-ttu-id="f948c-118">venceu</span><span class="sxs-lookup"><span data-stu-id="f948c-118">expired</span></span>|<span data-ttu-id="f948c-119">2 </span><span class="sxs-lookup"><span data-stu-id="f948c-119">2</span></span>|<span data-ttu-id="f948c-120">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="f948c-120">Token is expired.</span></span>|
|<span data-ttu-id="f948c-121">Inválido</span><span class="sxs-lookup"><span data-stu-id="f948c-121">invalid</span></span>|<span data-ttu-id="f948c-122">3 </span><span class="sxs-lookup"><span data-stu-id="f948c-122">3</span></span>|<span data-ttu-id="f948c-123">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="f948c-123">Token is invalid.</span></span>|
|<span data-ttu-id="f948c-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="f948c-124">assignedToExternalMDM</span></span>|<span data-ttu-id="f948c-125">4 </span><span class="sxs-lookup"><span data-stu-id="f948c-125">4</span></span>|<span data-ttu-id="f948c-126">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="f948c-126">Token is managed by another MDM Service.</span></span>|



