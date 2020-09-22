---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bdc4730684afb7856df0a29210b37f78bdb7ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042482"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="7f091-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="7f091-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="7f091-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f091-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f091-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f091-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f091-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f091-107">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="7f091-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="7f091-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7f091-108">Members</span></span>
|<span data-ttu-id="7f091-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7f091-109">Member</span></span>|<span data-ttu-id="7f091-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7f091-110">Value</span></span>|<span data-ttu-id="7f091-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f091-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f091-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7f091-112">notConfigured</span></span>|<span data-ttu-id="7f091-113">,0</span><span class="sxs-lookup"><span data-stu-id="7f091-113">0</span></span>|<span data-ttu-id="7f091-114">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="7f091-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="7f091-115">high</span><span class="sxs-lookup"><span data-stu-id="7f091-115">high</span></span>|<span data-ttu-id="7f091-116">1 </span><span class="sxs-lookup"><span data-stu-id="7f091-116">1</span></span>|<span data-ttu-id="7f091-117">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="7f091-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="7f091-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="7f091-118">highPlus</span></span>|<span data-ttu-id="7f091-119">2 </span><span class="sxs-lookup"><span data-stu-id="7f091-119">2</span></span>|<span data-ttu-id="7f091-120">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="7f091-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="7f091-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="7f091-121">zeroTolerance</span></span>|<span data-ttu-id="7f091-122">3 </span><span class="sxs-lookup"><span data-stu-id="7f091-122">3</span></span>|<span data-ttu-id="7f091-123">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="7f091-123">Zero tolerance blocks all unknown executables</span></span>|






