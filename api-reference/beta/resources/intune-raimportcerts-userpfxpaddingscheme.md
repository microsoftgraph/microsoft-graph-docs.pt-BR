---
title: tipo de enumeração userPfxPaddingScheme
description: Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0cbdc056c1dc0ea1aa73ae0cd96af428ce9f2bf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307162"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="1a347-103">tipo de enumeração userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="1a347-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="1a347-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a347-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a347-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a347-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a347-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a347-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a347-107">Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.</span><span class="sxs-lookup"><span data-stu-id="1a347-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="1a347-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1a347-108">Members</span></span>
|<span data-ttu-id="1a347-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1a347-109">Member</span></span>|<span data-ttu-id="1a347-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1a347-110">Value</span></span>|<span data-ttu-id="1a347-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a347-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a347-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="1a347-112">none</span></span>|<span data-ttu-id="1a347-113">,0</span><span class="sxs-lookup"><span data-stu-id="1a347-113">0</span></span>|<span data-ttu-id="1a347-114">Esquema de preenchimento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="1a347-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="1a347-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="1a347-115">pkcs1</span></span>|<span data-ttu-id="1a347-116">1</span><span class="sxs-lookup"><span data-stu-id="1a347-116">1</span></span>|<span data-ttu-id="1a347-117">Pkcs1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="1a347-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="1a347-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="1a347-118">oaepSha1</span></span>|<span data-ttu-id="1a347-119">duas</span><span class="sxs-lookup"><span data-stu-id="1a347-119">2</span></span>|<span data-ttu-id="1a347-120">OaepSha1 não tem mais suporte</span><span class="sxs-lookup"><span data-stu-id="1a347-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="1a347-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="1a347-121">oaepSha256</span></span>|<span data-ttu-id="1a347-122">3D</span><span class="sxs-lookup"><span data-stu-id="1a347-122">3</span></span>|<span data-ttu-id="1a347-123">Use o preenchimento OAEP SHA-256.</span><span class="sxs-lookup"><span data-stu-id="1a347-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="1a347-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="1a347-124">oaepSha384</span></span>|<span data-ttu-id="1a347-125">4 </span><span class="sxs-lookup"><span data-stu-id="1a347-125">4</span></span>|<span data-ttu-id="1a347-126">Use o preenchimento OAEP SHA-384.</span><span class="sxs-lookup"><span data-stu-id="1a347-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="1a347-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="1a347-127">oaepSha512</span></span>|<span data-ttu-id="1a347-128">5 </span><span class="sxs-lookup"><span data-stu-id="1a347-128">5</span></span>|<span data-ttu-id="1a347-129">Use o preenchimento OAEP SHA-512.</span><span class="sxs-lookup"><span data-stu-id="1a347-129">Use OAEP SHA-512 padding.</span></span>|




