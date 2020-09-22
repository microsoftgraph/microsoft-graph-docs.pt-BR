---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07a9441923e99089fc3dc2ebe9627972237207e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025274"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="427e3-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="427e3-103">vppTokenState enum type</span></span>

<span data-ttu-id="427e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="427e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="427e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="427e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="427e3-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="427e3-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="427e3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="427e3-107">Members</span></span>
|<span data-ttu-id="427e3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="427e3-108">Member</span></span>|<span data-ttu-id="427e3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="427e3-109">Value</span></span>|<span data-ttu-id="427e3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="427e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="427e3-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="427e3-111">unknown</span></span>|<span data-ttu-id="427e3-112">,0</span><span class="sxs-lookup"><span data-stu-id="427e3-112">0</span></span>|<span data-ttu-id="427e3-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="427e3-113">Default state.</span></span>|
|<span data-ttu-id="427e3-114">inválido</span><span class="sxs-lookup"><span data-stu-id="427e3-114">valid</span></span>|<span data-ttu-id="427e3-115">1 </span><span class="sxs-lookup"><span data-stu-id="427e3-115">1</span></span>|<span data-ttu-id="427e3-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="427e3-116">Token is valid.</span></span>|
|<span data-ttu-id="427e3-117">venceu</span><span class="sxs-lookup"><span data-stu-id="427e3-117">expired</span></span>|<span data-ttu-id="427e3-118">2 </span><span class="sxs-lookup"><span data-stu-id="427e3-118">2</span></span>|<span data-ttu-id="427e3-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="427e3-119">Token is expired.</span></span>|
|<span data-ttu-id="427e3-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="427e3-120">invalid</span></span>|<span data-ttu-id="427e3-121">3 </span><span class="sxs-lookup"><span data-stu-id="427e3-121">3</span></span>|<span data-ttu-id="427e3-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="427e3-122">Token is invalid.</span></span>|
|<span data-ttu-id="427e3-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="427e3-123">assignedToExternalMDM</span></span>|<span data-ttu-id="427e3-124">4 </span><span class="sxs-lookup"><span data-stu-id="427e3-124">4</span></span>|<span data-ttu-id="427e3-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="427e3-125">Token is managed by another MDM Service.</span></span>|









