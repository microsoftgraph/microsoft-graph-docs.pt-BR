---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 644b1d58a38d23d71a2fa56e7bfd5d678ffee76e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447994"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="6a142-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="6a142-103">vppTokenState enum type</span></span>

<span data-ttu-id="6a142-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a142-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a142-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a142-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a142-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6a142-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="6a142-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6a142-107">Members</span></span>
|<span data-ttu-id="6a142-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6a142-108">Member</span></span>|<span data-ttu-id="6a142-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6a142-109">Value</span></span>|<span data-ttu-id="6a142-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a142-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a142-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6a142-111">unknown</span></span>|<span data-ttu-id="6a142-112">,0</span><span class="sxs-lookup"><span data-stu-id="6a142-112">0</span></span>|<span data-ttu-id="6a142-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="6a142-113">Default state.</span></span>|
|<span data-ttu-id="6a142-114">inválido</span><span class="sxs-lookup"><span data-stu-id="6a142-114">valid</span></span>|<span data-ttu-id="6a142-115">1 </span><span class="sxs-lookup"><span data-stu-id="6a142-115">1</span></span>|<span data-ttu-id="6a142-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="6a142-116">Token is valid.</span></span>|
|<span data-ttu-id="6a142-117">venceu</span><span class="sxs-lookup"><span data-stu-id="6a142-117">expired</span></span>|<span data-ttu-id="6a142-118">2 </span><span class="sxs-lookup"><span data-stu-id="6a142-118">2</span></span>|<span data-ttu-id="6a142-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="6a142-119">Token is expired.</span></span>|
|<span data-ttu-id="6a142-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="6a142-120">invalid</span></span>|<span data-ttu-id="6a142-121">3 </span><span class="sxs-lookup"><span data-stu-id="6a142-121">3</span></span>|<span data-ttu-id="6a142-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="6a142-122">Token is invalid.</span></span>|
|<span data-ttu-id="6a142-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="6a142-123">assignedToExternalMDM</span></span>|<span data-ttu-id="6a142-124">4 </span><span class="sxs-lookup"><span data-stu-id="6a142-124">4</span></span>|<span data-ttu-id="6a142-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="6a142-125">Token is managed by another MDM Service.</span></span>|




