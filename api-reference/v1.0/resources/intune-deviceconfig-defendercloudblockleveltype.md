---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86d3da357b519ab3da0e4a4947ab933339aae134
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449086"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f3d5b-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="f3d5b-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="f3d5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3d5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3d5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3d5b-106">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="f3d5b-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="f3d5b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f3d5b-107">Members</span></span>
|<span data-ttu-id="f3d5b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f3d5b-108">Member</span></span>|<span data-ttu-id="f3d5b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f3d5b-109">Value</span></span>|<span data-ttu-id="f3d5b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3d5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d5b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f3d5b-111">notConfigured</span></span>|<span data-ttu-id="f3d5b-112">,0</span><span class="sxs-lookup"><span data-stu-id="f3d5b-112">0</span></span>|<span data-ttu-id="f3d5b-113">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="f3d5b-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f3d5b-114">high</span><span class="sxs-lookup"><span data-stu-id="f3d5b-114">high</span></span>|<span data-ttu-id="f3d5b-115">1</span><span class="sxs-lookup"><span data-stu-id="f3d5b-115">1</span></span>|<span data-ttu-id="f3d5b-116">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="f3d5b-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f3d5b-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="f3d5b-117">highPlus</span></span>|<span data-ttu-id="f3d5b-118">duas</span><span class="sxs-lookup"><span data-stu-id="f3d5b-118">2</span></span>|<span data-ttu-id="f3d5b-119">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="f3d5b-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f3d5b-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="f3d5b-120">zeroTolerance</span></span>|<span data-ttu-id="f3d5b-121">3D</span><span class="sxs-lookup"><span data-stu-id="f3d5b-121">3</span></span>|<span data-ttu-id="f3d5b-122">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f3d5b-122">Zero tolerance blocks all unknown executables</span></span>|







