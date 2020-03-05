---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 381f65c3f9a84c0d126fecd569bab72b48dcfc2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530184"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="6d8a8-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="6d8a8-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="6d8a8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d8a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d8a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d8a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d8a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d8a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d8a8-107">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="6d8a8-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="6d8a8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6d8a8-108">Members</span></span>
|<span data-ttu-id="6d8a8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6d8a8-109">Member</span></span>|<span data-ttu-id="6d8a8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6d8a8-110">Value</span></span>|<span data-ttu-id="6d8a8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d8a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d8a8-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6d8a8-112">notConfigured</span></span>|<span data-ttu-id="6d8a8-113">,0</span><span class="sxs-lookup"><span data-stu-id="6d8a8-113">0</span></span>|<span data-ttu-id="6d8a8-114">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="6d8a8-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="6d8a8-115">high</span><span class="sxs-lookup"><span data-stu-id="6d8a8-115">high</span></span>|<span data-ttu-id="6d8a8-116">1 </span><span class="sxs-lookup"><span data-stu-id="6d8a8-116">1</span></span>|<span data-ttu-id="6d8a8-117">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="6d8a8-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="6d8a8-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="6d8a8-118">highPlus</span></span>|<span data-ttu-id="6d8a8-119">2 </span><span class="sxs-lookup"><span data-stu-id="6d8a8-119">2</span></span>|<span data-ttu-id="6d8a8-120">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="6d8a8-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="6d8a8-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="6d8a8-121">zeroTolerance</span></span>|<span data-ttu-id="6d8a8-122">3 </span><span class="sxs-lookup"><span data-stu-id="6d8a8-122">3</span></span>|<span data-ttu-id="6d8a8-123">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="6d8a8-123">Zero tolerance blocks all unknown executables</span></span>|



