---
title: enumeração fileHashType
description: Enum para tipos de arquivo de hash.
ms.openlocfilehash: fbaa390ee8c543d2ed7c77cc05a11b519df0da9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033837"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="d98c4-103">enumeração fileHashType</span><span class="sxs-lookup"><span data-stu-id="d98c4-103">fileHashType enum</span></span>

> <span data-ttu-id="d98c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d98c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d98c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d98c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d98c4-106">Enum para tipos de arquivo de hash.</span><span class="sxs-lookup"><span data-stu-id="d98c4-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="d98c4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d98c4-107">Members</span></span>

|<span data-ttu-id="d98c4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d98c4-108">Member</span></span>|<span data-ttu-id="d98c4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d98c4-109">Value</span></span>|<span data-ttu-id="d98c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d98c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98c4-111">unknown</span><span class="sxs-lookup"><span data-stu-id="d98c4-111">unknown</span></span>|<span data-ttu-id="d98c4-112">0</span><span class="sxs-lookup"><span data-stu-id="d98c4-112">0</span></span>|<span data-ttu-id="d98c4-113">Tipo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d98c4-113">Unknown type.</span></span>|
|<span data-ttu-id="d98c4-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="d98c4-114">sha1</span></span>|<span data-ttu-id="d98c4-115">1</span><span class="sxs-lookup"><span data-stu-id="d98c4-115">1</span></span>|<span data-ttu-id="d98c4-116">Tipo de hash SHA1.</span><span class="sxs-lookup"><span data-stu-id="d98c4-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="d98c4-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="d98c4-117">sha256</span></span>|<span data-ttu-id="d98c4-118">2</span><span class="sxs-lookup"><span data-stu-id="d98c4-118">2</span></span>| <span data-ttu-id="d98c4-119">Tipo de hash SHA256.</span><span class="sxs-lookup"><span data-stu-id="d98c4-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="d98c4-120">MD5</span><span class="sxs-lookup"><span data-stu-id="d98c4-120">md5</span></span>|<span data-ttu-id="d98c4-121">3</span><span class="sxs-lookup"><span data-stu-id="d98c4-121">3</span></span>| <span data-ttu-id="d98c4-122">Tipo de hash MD5.</span><span class="sxs-lookup"><span data-stu-id="d98c4-122">MD5 hash type.</span></span>|
|<span data-ttu-id="d98c4-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="d98c4-123">authenticodeHash256</span></span>|<span data-ttu-id="d98c4-124">4</span><span class="sxs-lookup"><span data-stu-id="d98c4-124">4</span></span>| <span data-ttu-id="d98c4-125">Tipo de hash AuthenticodeHash256.</span><span class="sxs-lookup"><span data-stu-id="d98c4-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="d98c4-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="d98c4-126">lsHash</span></span>|<span data-ttu-id="d98c4-127">5</span><span class="sxs-lookup"><span data-stu-id="d98c4-127">5</span></span>| <span data-ttu-id="d98c4-128">Tipo de hash LsHash.</span><span class="sxs-lookup"><span data-stu-id="d98c4-128">LsHash hash type.</span></span>|
|<span data-ttu-id="d98c4-129">ctph</span><span class="sxs-lookup"><span data-stu-id="d98c4-129">ctph</span></span>|<span data-ttu-id="d98c4-130">6</span><span class="sxs-lookup"><span data-stu-id="d98c4-130">6</span></span>| <span data-ttu-id="d98c4-131">Tipo de hash CTPH.</span><span class="sxs-lookup"><span data-stu-id="d98c4-131">CTPH hash type.</span></span>|
|<span data-ttu-id="d98c4-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="d98c4-132">peSha1</span></span>|<span data-ttu-id="d98c4-133">7</span><span class="sxs-lookup"><span data-stu-id="d98c4-133">7</span></span>| <span data-ttu-id="d98c4-134">Tipo de hash PESHA1.</span><span class="sxs-lookup"><span data-stu-id="d98c4-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="d98c4-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="d98c4-135">peSha256</span></span>|<span data-ttu-id="d98c4-136">8</span><span class="sxs-lookup"><span data-stu-id="d98c4-136">8</span></span>| <span data-ttu-id="d98c4-137">Tipo de hash PESHA256.</span><span class="sxs-lookup"><span data-stu-id="d98c4-137">PESHA256 hash type.</span></span>|
