---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d0c5db4ffaac3a08edad42e7529b62337bf0ed52
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369357"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="b9a62-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b9a62-103">vppTokenState enum type</span></span>

> <span data-ttu-id="b9a62-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9a62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9a62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9a62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a62-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b9a62-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="b9a62-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b9a62-107">Members</span></span>
|<span data-ttu-id="b9a62-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b9a62-108">Member</span></span>|<span data-ttu-id="b9a62-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b9a62-109">Value</span></span>|<span data-ttu-id="b9a62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a62-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="b9a62-111">unknown</span></span>|<span data-ttu-id="b9a62-112">,0</span><span class="sxs-lookup"><span data-stu-id="b9a62-112">0</span></span>|<span data-ttu-id="b9a62-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="b9a62-113">Default state.</span></span>|
|<span data-ttu-id="b9a62-114">inválido</span><span class="sxs-lookup"><span data-stu-id="b9a62-114">valid</span></span>|<span data-ttu-id="b9a62-115">1</span><span class="sxs-lookup"><span data-stu-id="b9a62-115">1</span></span>|<span data-ttu-id="b9a62-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="b9a62-116">Token is valid.</span></span>|
|<span data-ttu-id="b9a62-117">venceu</span><span class="sxs-lookup"><span data-stu-id="b9a62-117">expired</span></span>|<span data-ttu-id="b9a62-118">duas</span><span class="sxs-lookup"><span data-stu-id="b9a62-118">2</span></span>|<span data-ttu-id="b9a62-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="b9a62-119">Token is expired.</span></span>|
|<span data-ttu-id="b9a62-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="b9a62-120">invalid</span></span>|<span data-ttu-id="b9a62-121">3D</span><span class="sxs-lookup"><span data-stu-id="b9a62-121">3</span></span>|<span data-ttu-id="b9a62-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="b9a62-122">Token is invalid.</span></span>|
|<span data-ttu-id="b9a62-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="b9a62-123">assignedToExternalMDM</span></span>|<span data-ttu-id="b9a62-124">quatro</span><span class="sxs-lookup"><span data-stu-id="b9a62-124">4</span></span>|<span data-ttu-id="b9a62-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="b9a62-125">Token is managed by another MDM Service.</span></span>|



