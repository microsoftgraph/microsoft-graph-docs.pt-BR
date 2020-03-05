---
title: tipo de enumeração userPfxPaddingScheme
description: Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f1d2b51ce966caf923e15e39694db616b639c441
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523925"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="809db-103">tipo de enumeração userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="809db-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="809db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="809db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="809db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="809db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="809db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="809db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809db-107">Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.</span><span class="sxs-lookup"><span data-stu-id="809db-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="809db-108">Membros</span><span class="sxs-lookup"><span data-stu-id="809db-108">Members</span></span>
|<span data-ttu-id="809db-109">Membro</span><span class="sxs-lookup"><span data-stu-id="809db-109">Member</span></span>|<span data-ttu-id="809db-110">Valor</span><span class="sxs-lookup"><span data-stu-id="809db-110">Value</span></span>|<span data-ttu-id="809db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="809db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="809db-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="809db-112">none</span></span>|<span data-ttu-id="809db-113">,0</span><span class="sxs-lookup"><span data-stu-id="809db-113">0</span></span>|<span data-ttu-id="809db-114">Esquema de preenchimento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="809db-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="809db-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="809db-115">pkcs1</span></span>|<span data-ttu-id="809db-116">1 </span><span class="sxs-lookup"><span data-stu-id="809db-116">1</span></span>|<span data-ttu-id="809db-117">Pkcs1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="809db-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="809db-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="809db-118">oaepSha1</span></span>|<span data-ttu-id="809db-119">2 </span><span class="sxs-lookup"><span data-stu-id="809db-119">2</span></span>|<span data-ttu-id="809db-120">OaepSha1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="809db-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="809db-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="809db-121">oaepSha256</span></span>|<span data-ttu-id="809db-122">3 </span><span class="sxs-lookup"><span data-stu-id="809db-122">3</span></span>|<span data-ttu-id="809db-123">Use o preenchimento OAEP SHA-256.</span><span class="sxs-lookup"><span data-stu-id="809db-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="809db-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="809db-124">oaepSha384</span></span>|<span data-ttu-id="809db-125">4 </span><span class="sxs-lookup"><span data-stu-id="809db-125">4</span></span>|<span data-ttu-id="809db-126">Use o preenchimento OAEP SHA-384.</span><span class="sxs-lookup"><span data-stu-id="809db-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="809db-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="809db-127">oaepSha512</span></span>|<span data-ttu-id="809db-128">5 </span><span class="sxs-lookup"><span data-stu-id="809db-128">5</span></span>|<span data-ttu-id="809db-129">Use o preenchimento OAEP SHA-512.</span><span class="sxs-lookup"><span data-stu-id="809db-129">Use OAEP SHA-512 padding.</span></span>|



