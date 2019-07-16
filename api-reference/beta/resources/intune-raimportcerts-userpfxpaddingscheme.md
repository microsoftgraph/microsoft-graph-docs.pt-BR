---
title: tipo de enumeração userPfxPaddingScheme
description: Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a079075d3e0a44a773c854df55df1635d54584c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739271"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="e9e70-103">tipo de enumeração userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="e9e70-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="e9e70-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9e70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9e70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9e70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9e70-106">Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.</span><span class="sxs-lookup"><span data-stu-id="e9e70-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="e9e70-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e9e70-107">Members</span></span>
|<span data-ttu-id="e9e70-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e9e70-108">Member</span></span>|<span data-ttu-id="e9e70-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e9e70-109">Value</span></span>|<span data-ttu-id="e9e70-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9e70-111">none</span><span class="sxs-lookup"><span data-stu-id="e9e70-111">none</span></span>|<span data-ttu-id="e9e70-112">,0</span><span class="sxs-lookup"><span data-stu-id="e9e70-112">0</span></span>|<span data-ttu-id="e9e70-113">Nenhum preenchimento é usado.</span><span class="sxs-lookup"><span data-stu-id="e9e70-113">No padding used.</span></span>|
|<span data-ttu-id="e9e70-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="e9e70-114">pkcs1</span></span>|<span data-ttu-id="e9e70-115">1</span><span class="sxs-lookup"><span data-stu-id="e9e70-115">1</span></span>|<span data-ttu-id="e9e70-116">Usar preenchimento PKCS # 1.</span><span class="sxs-lookup"><span data-stu-id="e9e70-116">Use PKCS#1 padding.</span></span>|
|<span data-ttu-id="e9e70-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="e9e70-117">oaepSha1</span></span>|<span data-ttu-id="e9e70-118">duas</span><span class="sxs-lookup"><span data-stu-id="e9e70-118">2</span></span>|<span data-ttu-id="e9e70-119">Use o enchimento OAEP SHA-1.</span><span class="sxs-lookup"><span data-stu-id="e9e70-119">Use OAEP SHA-1 padding.</span></span>|
|<span data-ttu-id="e9e70-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="e9e70-120">oaepSha256</span></span>|<span data-ttu-id="e9e70-121">3D</span><span class="sxs-lookup"><span data-stu-id="e9e70-121">3</span></span>|<span data-ttu-id="e9e70-122">Use o preenchimento OAEP SHA-256.</span><span class="sxs-lookup"><span data-stu-id="e9e70-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="e9e70-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="e9e70-123">oaepSha384</span></span>|<span data-ttu-id="e9e70-124">quatro</span><span class="sxs-lookup"><span data-stu-id="e9e70-124">4</span></span>|<span data-ttu-id="e9e70-125">Use o preenchimento OAEP SHA-384.</span><span class="sxs-lookup"><span data-stu-id="e9e70-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="e9e70-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="e9e70-126">oaepSha512</span></span>|<span data-ttu-id="e9e70-127">0,5</span><span class="sxs-lookup"><span data-stu-id="e9e70-127">5</span></span>|<span data-ttu-id="e9e70-128">Use o preenchimento OAEP SHA-512.</span><span class="sxs-lookup"><span data-stu-id="e9e70-128">Use OAEP SHA-512 padding.</span></span>|





