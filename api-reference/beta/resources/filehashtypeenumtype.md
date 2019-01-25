---
title: enumeração fileHashType
description: Enum para tipos de arquivo de hash.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518377"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="03533-103">enumeração fileHashType</span><span class="sxs-lookup"><span data-stu-id="03533-103">fileHashType enum</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03533-104">Enum para tipos de arquivo de hash.</span><span class="sxs-lookup"><span data-stu-id="03533-104">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="03533-105">Membros</span><span class="sxs-lookup"><span data-stu-id="03533-105">Members</span></span>

|<span data-ttu-id="03533-106">Membro</span><span class="sxs-lookup"><span data-stu-id="03533-106">Member</span></span>|<span data-ttu-id="03533-107">Valor</span><span class="sxs-lookup"><span data-stu-id="03533-107">Value</span></span>|<span data-ttu-id="03533-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="03533-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03533-109">unknown</span><span class="sxs-lookup"><span data-stu-id="03533-109">unknown</span></span>|<span data-ttu-id="03533-110">.0</span><span class="sxs-lookup"><span data-stu-id="03533-110">0</span></span>|<span data-ttu-id="03533-111">Tipo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="03533-111">Unknown type.</span></span>|
|<span data-ttu-id="03533-112">SHA1</span><span class="sxs-lookup"><span data-stu-id="03533-112">sha1</span></span>|<span data-ttu-id="03533-113">-1</span><span class="sxs-lookup"><span data-stu-id="03533-113">1</span></span>|<span data-ttu-id="03533-114">Tipo de hash SHA1.</span><span class="sxs-lookup"><span data-stu-id="03533-114">SHA1 hash type.</span></span>|
|<span data-ttu-id="03533-115">SHA256</span><span class="sxs-lookup"><span data-stu-id="03533-115">sha256</span></span>|<span data-ttu-id="03533-116">-2</span><span class="sxs-lookup"><span data-stu-id="03533-116">2</span></span>| <span data-ttu-id="03533-117">Tipo de hash SHA256.</span><span class="sxs-lookup"><span data-stu-id="03533-117">SHA256 hash type.</span></span>|
|<span data-ttu-id="03533-118">MD5</span><span class="sxs-lookup"><span data-stu-id="03533-118">md5</span></span>|<span data-ttu-id="03533-119">-3</span><span class="sxs-lookup"><span data-stu-id="03533-119">3</span></span>| <span data-ttu-id="03533-120">Tipo de hash MD5.</span><span class="sxs-lookup"><span data-stu-id="03533-120">MD5 hash type.</span></span>|
|<span data-ttu-id="03533-121">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="03533-121">authenticodeHash256</span></span>|<span data-ttu-id="03533-122">4\*</span><span class="sxs-lookup"><span data-stu-id="03533-122">4</span></span>| <span data-ttu-id="03533-123">Tipo de hash AuthenticodeHash256.</span><span class="sxs-lookup"><span data-stu-id="03533-123">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="03533-124">lsHash</span><span class="sxs-lookup"><span data-stu-id="03533-124">lsHash</span></span>|<span data-ttu-id="03533-125">.5</span><span class="sxs-lookup"><span data-stu-id="03533-125">5</span></span>| <span data-ttu-id="03533-126">Tipo de hash LsHash.</span><span class="sxs-lookup"><span data-stu-id="03533-126">LsHash hash type.</span></span>|
|<span data-ttu-id="03533-127">ctph</span><span class="sxs-lookup"><span data-stu-id="03533-127">ctph</span></span>|<span data-ttu-id="03533-128">-6</span><span class="sxs-lookup"><span data-stu-id="03533-128">6</span></span>| <span data-ttu-id="03533-129">Tipo de hash CTPH.</span><span class="sxs-lookup"><span data-stu-id="03533-129">CTPH hash type.</span></span>|
|<span data-ttu-id="03533-130">peSha1</span><span class="sxs-lookup"><span data-stu-id="03533-130">peSha1</span></span>|<span data-ttu-id="03533-131">-7</span><span class="sxs-lookup"><span data-stu-id="03533-131">7</span></span>| <span data-ttu-id="03533-132">Tipo de hash PESHA1.</span><span class="sxs-lookup"><span data-stu-id="03533-132">PESHA1 hash type.</span></span>|
|<span data-ttu-id="03533-133">peSha256</span><span class="sxs-lookup"><span data-stu-id="03533-133">peSha256</span></span>|<span data-ttu-id="03533-134">8\*</span><span class="sxs-lookup"><span data-stu-id="03533-134">8</span></span>| <span data-ttu-id="03533-135">Tipo de hash PESHA256.</span><span class="sxs-lookup"><span data-stu-id="03533-135">PESHA256 hash type.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
