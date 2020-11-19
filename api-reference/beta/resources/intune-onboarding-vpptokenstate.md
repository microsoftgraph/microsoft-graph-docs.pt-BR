---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8a159a5a2e359cef6978df44a8f40a1d664dfa48
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259400"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="0fb17-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="0fb17-103">vppTokenState enum type</span></span>

<span data-ttu-id="0fb17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fb17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fb17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fb17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb17-107">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0fb17-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="0fb17-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0fb17-108">Members</span></span>
|<span data-ttu-id="0fb17-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0fb17-109">Member</span></span>|<span data-ttu-id="0fb17-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0fb17-110">Value</span></span>|<span data-ttu-id="0fb17-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb17-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="0fb17-112">unknown</span></span>|<span data-ttu-id="0fb17-113">,0</span><span class="sxs-lookup"><span data-stu-id="0fb17-113">0</span></span>|<span data-ttu-id="0fb17-114">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="0fb17-114">Default state.</span></span>|
|<span data-ttu-id="0fb17-115">inválido</span><span class="sxs-lookup"><span data-stu-id="0fb17-115">valid</span></span>|<span data-ttu-id="0fb17-116">1</span><span class="sxs-lookup"><span data-stu-id="0fb17-116">1</span></span>|<span data-ttu-id="0fb17-117">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="0fb17-117">Token is valid.</span></span>|
|<span data-ttu-id="0fb17-118">venceu</span><span class="sxs-lookup"><span data-stu-id="0fb17-118">expired</span></span>|<span data-ttu-id="0fb17-119">duas</span><span class="sxs-lookup"><span data-stu-id="0fb17-119">2</span></span>|<span data-ttu-id="0fb17-120">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="0fb17-120">Token is expired.</span></span>|
|<span data-ttu-id="0fb17-121">Inválido</span><span class="sxs-lookup"><span data-stu-id="0fb17-121">invalid</span></span>|<span data-ttu-id="0fb17-122">3D</span><span class="sxs-lookup"><span data-stu-id="0fb17-122">3</span></span>|<span data-ttu-id="0fb17-123">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="0fb17-123">Token is invalid.</span></span>|
|<span data-ttu-id="0fb17-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="0fb17-124">assignedToExternalMDM</span></span>|<span data-ttu-id="0fb17-125">4 </span><span class="sxs-lookup"><span data-stu-id="0fb17-125">4</span></span>|<span data-ttu-id="0fb17-126">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="0fb17-126">Token is managed by another MDM Service.</span></span>|
|<span data-ttu-id="0fb17-127">duplicateLocationId</span><span class="sxs-lookup"><span data-stu-id="0fb17-127">duplicateLocationId</span></span>|<span data-ttu-id="0fb17-128">5 </span><span class="sxs-lookup"><span data-stu-id="0fb17-128">5</span></span>|<span data-ttu-id="0fb17-129">O token é associado ao mesmo local de outro token na conta.</span><span class="sxs-lookup"><span data-stu-id="0fb17-129">Token is associated with the same location as another token on the account.</span></span>|




