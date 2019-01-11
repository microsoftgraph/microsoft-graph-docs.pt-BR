---
title: enumeração fileHashType
description: Enum para tipos de arquivo de hash.
localization_priority: Normal
ms.openlocfilehash: e1c31aaea6c8cea40817efea61dc8654d3d17fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816326"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="7a14d-103">enumeração fileHashType</span><span class="sxs-lookup"><span data-stu-id="7a14d-103">fileHashType enum</span></span>

> <span data-ttu-id="7a14d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a14d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a14d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a14d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a14d-106">Enum para tipos de arquivo de hash.</span><span class="sxs-lookup"><span data-stu-id="7a14d-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="7a14d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7a14d-107">Members</span></span>

|<span data-ttu-id="7a14d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7a14d-108">Member</span></span>|<span data-ttu-id="7a14d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7a14d-109">Value</span></span>|<span data-ttu-id="7a14d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a14d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a14d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="7a14d-111">unknown</span></span>|<span data-ttu-id="7a14d-112">0</span><span class="sxs-lookup"><span data-stu-id="7a14d-112">0</span></span>|<span data-ttu-id="7a14d-113">Tipo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7a14d-113">Unknown type.</span></span>|
|<span data-ttu-id="7a14d-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="7a14d-114">sha1</span></span>|<span data-ttu-id="7a14d-115">1</span><span class="sxs-lookup"><span data-stu-id="7a14d-115">1</span></span>|<span data-ttu-id="7a14d-116">Tipo de hash SHA1.</span><span class="sxs-lookup"><span data-stu-id="7a14d-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="7a14d-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="7a14d-117">sha256</span></span>|<span data-ttu-id="7a14d-118">2</span><span class="sxs-lookup"><span data-stu-id="7a14d-118">2</span></span>| <span data-ttu-id="7a14d-119">Tipo de hash SHA256.</span><span class="sxs-lookup"><span data-stu-id="7a14d-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="7a14d-120">MD5</span><span class="sxs-lookup"><span data-stu-id="7a14d-120">md5</span></span>|<span data-ttu-id="7a14d-121">3</span><span class="sxs-lookup"><span data-stu-id="7a14d-121">3</span></span>| <span data-ttu-id="7a14d-122">Tipo de hash MD5.</span><span class="sxs-lookup"><span data-stu-id="7a14d-122">MD5 hash type.</span></span>|
|<span data-ttu-id="7a14d-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="7a14d-123">authenticodeHash256</span></span>|<span data-ttu-id="7a14d-124">4</span><span class="sxs-lookup"><span data-stu-id="7a14d-124">4</span></span>| <span data-ttu-id="7a14d-125">Tipo de hash AuthenticodeHash256.</span><span class="sxs-lookup"><span data-stu-id="7a14d-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="7a14d-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="7a14d-126">lsHash</span></span>|<span data-ttu-id="7a14d-127">5</span><span class="sxs-lookup"><span data-stu-id="7a14d-127">5</span></span>| <span data-ttu-id="7a14d-128">Tipo de hash LsHash.</span><span class="sxs-lookup"><span data-stu-id="7a14d-128">LsHash hash type.</span></span>|
|<span data-ttu-id="7a14d-129">ctph</span><span class="sxs-lookup"><span data-stu-id="7a14d-129">ctph</span></span>|<span data-ttu-id="7a14d-130">6</span><span class="sxs-lookup"><span data-stu-id="7a14d-130">6</span></span>| <span data-ttu-id="7a14d-131">Tipo de hash CTPH.</span><span class="sxs-lookup"><span data-stu-id="7a14d-131">CTPH hash type.</span></span>|
|<span data-ttu-id="7a14d-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="7a14d-132">peSha1</span></span>|<span data-ttu-id="7a14d-133">7</span><span class="sxs-lookup"><span data-stu-id="7a14d-133">7</span></span>| <span data-ttu-id="7a14d-134">Tipo de hash PESHA1.</span><span class="sxs-lookup"><span data-stu-id="7a14d-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="7a14d-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="7a14d-135">peSha256</span></span>|<span data-ttu-id="7a14d-136">8</span><span class="sxs-lookup"><span data-stu-id="7a14d-136">8</span></span>| <span data-ttu-id="7a14d-137">Tipo de hash PESHA256.</span><span class="sxs-lookup"><span data-stu-id="7a14d-137">PESHA256 hash type.</span></span>|
