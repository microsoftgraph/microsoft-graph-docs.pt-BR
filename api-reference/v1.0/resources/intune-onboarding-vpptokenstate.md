---
title: Tipo denum vppTokenState
description: Estados possíveis associados a um token do Programa de Compra de Volume da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26492a317a5fe147a49cc8cda7103fa492704deb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755697"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="0a091-103">Tipo denum vppTokenState</span><span class="sxs-lookup"><span data-stu-id="0a091-103">vppTokenState enum type</span></span>

<span data-ttu-id="0a091-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a091-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a091-106">Estados possíveis associados a um token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="0a091-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="0a091-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0a091-107">Members</span></span>
|<span data-ttu-id="0a091-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0a091-108">Member</span></span>|<span data-ttu-id="0a091-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0a091-109">Value</span></span>|<span data-ttu-id="0a091-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a091-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a091-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="0a091-111">unknown</span></span>|<span data-ttu-id="0a091-112">0</span><span class="sxs-lookup"><span data-stu-id="0a091-112">0</span></span>|<span data-ttu-id="0a091-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="0a091-113">Default state.</span></span>|
|<span data-ttu-id="0a091-114">valid</span><span class="sxs-lookup"><span data-stu-id="0a091-114">valid</span></span>|<span data-ttu-id="0a091-115">1</span><span class="sxs-lookup"><span data-stu-id="0a091-115">1</span></span>|<span data-ttu-id="0a091-116">Token é válido.</span><span class="sxs-lookup"><span data-stu-id="0a091-116">Token is valid.</span></span>|
|<span data-ttu-id="0a091-117">expirado</span><span class="sxs-lookup"><span data-stu-id="0a091-117">expired</span></span>|<span data-ttu-id="0a091-118">2</span><span class="sxs-lookup"><span data-stu-id="0a091-118">2</span></span>|<span data-ttu-id="0a091-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="0a091-119">Token is expired.</span></span>|
|<span data-ttu-id="0a091-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="0a091-120">invalid</span></span>|<span data-ttu-id="0a091-121">3</span><span class="sxs-lookup"><span data-stu-id="0a091-121">3</span></span>|<span data-ttu-id="0a091-122">Token é inválido.</span><span class="sxs-lookup"><span data-stu-id="0a091-122">Token is invalid.</span></span>|
|<span data-ttu-id="0a091-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="0a091-123">assignedToExternalMDM</span></span>|<span data-ttu-id="0a091-124">4 </span><span class="sxs-lookup"><span data-stu-id="0a091-124">4</span></span>|<span data-ttu-id="0a091-125">Token é gerenciado por outro Serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="0a091-125">Token is managed by another MDM Service.</span></span>|




