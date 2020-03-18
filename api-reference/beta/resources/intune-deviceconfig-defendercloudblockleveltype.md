---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3afc9a0bdf5d25c4496cb2dcf4a7ef013ac0785d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795615"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="82241-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="82241-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="82241-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82241-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82241-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82241-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82241-106">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="82241-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="82241-107">Membros</span><span class="sxs-lookup"><span data-stu-id="82241-107">Members</span></span>
|<span data-ttu-id="82241-108">Membro</span><span class="sxs-lookup"><span data-stu-id="82241-108">Member</span></span>|<span data-ttu-id="82241-109">Valor</span><span class="sxs-lookup"><span data-stu-id="82241-109">Value</span></span>|<span data-ttu-id="82241-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82241-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82241-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="82241-111">notConfigured</span></span>|<span data-ttu-id="82241-112">,0</span><span class="sxs-lookup"><span data-stu-id="82241-112">0</span></span>|<span data-ttu-id="82241-113">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="82241-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="82241-114">high</span><span class="sxs-lookup"><span data-stu-id="82241-114">high</span></span>|<span data-ttu-id="82241-115">1</span><span class="sxs-lookup"><span data-stu-id="82241-115">1</span></span>|<span data-ttu-id="82241-116">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="82241-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="82241-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="82241-117">highPlus</span></span>|<span data-ttu-id="82241-118">duas</span><span class="sxs-lookup"><span data-stu-id="82241-118">2</span></span>|<span data-ttu-id="82241-119">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="82241-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="82241-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="82241-120">zeroTolerance</span></span>|<span data-ttu-id="82241-121">3D</span><span class="sxs-lookup"><span data-stu-id="82241-121">3</span></span>|<span data-ttu-id="82241-122">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="82241-122">Zero tolerance blocks all unknown executables</span></span>|



