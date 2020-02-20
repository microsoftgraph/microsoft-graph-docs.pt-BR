---
title: tipo de enumeração userPfxPaddingScheme
description: Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6b04dcd01d21ace78368411524067f83db3bc93a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163546"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="5e80e-103">tipo de enumeração userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="5e80e-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="5e80e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e80e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e80e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e80e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e80e-106">Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.</span><span class="sxs-lookup"><span data-stu-id="5e80e-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="5e80e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5e80e-107">Members</span></span>
|<span data-ttu-id="5e80e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5e80e-108">Member</span></span>|<span data-ttu-id="5e80e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5e80e-109">Value</span></span>|<span data-ttu-id="5e80e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e80e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e80e-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="5e80e-111">none</span></span>|<span data-ttu-id="5e80e-112">,0</span><span class="sxs-lookup"><span data-stu-id="5e80e-112">0</span></span>|<span data-ttu-id="5e80e-113">Esquema de preenchimento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5e80e-113">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="5e80e-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="5e80e-114">pkcs1</span></span>|<span data-ttu-id="5e80e-115">1</span><span class="sxs-lookup"><span data-stu-id="5e80e-115">1</span></span>|<span data-ttu-id="5e80e-116">Pkcs1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="5e80e-116">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="5e80e-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="5e80e-117">oaepSha1</span></span>|<span data-ttu-id="5e80e-118">duas</span><span class="sxs-lookup"><span data-stu-id="5e80e-118">2</span></span>|<span data-ttu-id="5e80e-119">OaepSha1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="5e80e-119">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="5e80e-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="5e80e-120">oaepSha256</span></span>|<span data-ttu-id="5e80e-121">3D</span><span class="sxs-lookup"><span data-stu-id="5e80e-121">3</span></span>|<span data-ttu-id="5e80e-122">Use o preenchimento OAEP SHA-256.</span><span class="sxs-lookup"><span data-stu-id="5e80e-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="5e80e-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="5e80e-123">oaepSha384</span></span>|<span data-ttu-id="5e80e-124">quatro</span><span class="sxs-lookup"><span data-stu-id="5e80e-124">4</span></span>|<span data-ttu-id="5e80e-125">Use o preenchimento OAEP SHA-384.</span><span class="sxs-lookup"><span data-stu-id="5e80e-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="5e80e-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="5e80e-126">oaepSha512</span></span>|<span data-ttu-id="5e80e-127">0,5</span><span class="sxs-lookup"><span data-stu-id="5e80e-127">5</span></span>|<span data-ttu-id="5e80e-128">Use o preenchimento OAEP SHA-512.</span><span class="sxs-lookup"><span data-stu-id="5e80e-128">Use OAEP SHA-512 padding.</span></span>|



