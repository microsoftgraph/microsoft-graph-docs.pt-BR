---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c00ae796101131456db7206b80e4b6d8999fb86a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729753"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="fe3ae-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="fe3ae-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="fe3ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe3ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe3ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe3ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe3ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3ae-107">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="fe3ae-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="fe3ae-108">Membros</span><span class="sxs-lookup"><span data-stu-id="fe3ae-108">Members</span></span>
|<span data-ttu-id="fe3ae-109">Membro</span><span class="sxs-lookup"><span data-stu-id="fe3ae-109">Member</span></span>|<span data-ttu-id="fe3ae-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fe3ae-110">Value</span></span>|<span data-ttu-id="fe3ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe3ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3ae-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fe3ae-112">notConfigured</span></span>|<span data-ttu-id="fe3ae-113">,0</span><span class="sxs-lookup"><span data-stu-id="fe3ae-113">0</span></span>|<span data-ttu-id="fe3ae-114">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="fe3ae-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="fe3ae-115">high</span><span class="sxs-lookup"><span data-stu-id="fe3ae-115">high</span></span>|<span data-ttu-id="fe3ae-116">1</span><span class="sxs-lookup"><span data-stu-id="fe3ae-116">1</span></span>|<span data-ttu-id="fe3ae-117">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="fe3ae-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="fe3ae-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="fe3ae-118">highPlus</span></span>|<span data-ttu-id="fe3ae-119">duas</span><span class="sxs-lookup"><span data-stu-id="fe3ae-119">2</span></span>|<span data-ttu-id="fe3ae-120">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="fe3ae-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="fe3ae-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="fe3ae-121">zeroTolerance</span></span>|<span data-ttu-id="fe3ae-122">3D</span><span class="sxs-lookup"><span data-stu-id="fe3ae-122">3</span></span>|<span data-ttu-id="fe3ae-123">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="fe3ae-123">Zero tolerance blocks all unknown executables</span></span>|





