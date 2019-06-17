---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f798e4b7572cc2593d0d742ecbdebf81d65507d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979862"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="e0cbb-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="e0cbb-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="e0cbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0cbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0cbb-106">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="e0cbb-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="e0cbb-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e0cbb-107">Members</span></span>
|<span data-ttu-id="e0cbb-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e0cbb-108">Member</span></span>|<span data-ttu-id="e0cbb-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e0cbb-109">Value</span></span>|<span data-ttu-id="e0cbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0cbb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0cbb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e0cbb-111">notConfigured</span></span>|<span data-ttu-id="e0cbb-112">,0</span><span class="sxs-lookup"><span data-stu-id="e0cbb-112">0</span></span>|<span data-ttu-id="e0cbb-113">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="e0cbb-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="e0cbb-114">high</span><span class="sxs-lookup"><span data-stu-id="e0cbb-114">high</span></span>|<span data-ttu-id="e0cbb-115">1</span><span class="sxs-lookup"><span data-stu-id="e0cbb-115">1</span></span>|<span data-ttu-id="e0cbb-116">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="e0cbb-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="e0cbb-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="e0cbb-117">highPlus</span></span>|<span data-ttu-id="e0cbb-118">duas</span><span class="sxs-lookup"><span data-stu-id="e0cbb-118">2</span></span>|<span data-ttu-id="e0cbb-119">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="e0cbb-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="e0cbb-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="e0cbb-120">zeroTolerance</span></span>|<span data-ttu-id="e0cbb-121">3D</span><span class="sxs-lookup"><span data-stu-id="e0cbb-121">3</span></span>|<span data-ttu-id="e0cbb-122">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="e0cbb-122">Zero tolerance blocks all unknown executables</span></span>|





