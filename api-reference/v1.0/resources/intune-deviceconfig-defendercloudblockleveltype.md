---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908ebaef963b4c7d8baaf8f1cb0ecfb316d33ad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031875"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="6a49e-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="6a49e-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="6a49e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a49e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a49e-105">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="6a49e-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="6a49e-106">Membros</span><span class="sxs-lookup"><span data-stu-id="6a49e-106">Members</span></span>
|<span data-ttu-id="6a49e-107">Membro</span><span class="sxs-lookup"><span data-stu-id="6a49e-107">Member</span></span>|<span data-ttu-id="6a49e-108">Valor</span><span class="sxs-lookup"><span data-stu-id="6a49e-108">Value</span></span>|<span data-ttu-id="6a49e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a49e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a49e-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6a49e-110">notConfigured</span></span>|<span data-ttu-id="6a49e-111">,0</span><span class="sxs-lookup"><span data-stu-id="6a49e-111">0</span></span>|<span data-ttu-id="6a49e-112">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="6a49e-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="6a49e-113">high</span><span class="sxs-lookup"><span data-stu-id="6a49e-113">high</span></span>|<span data-ttu-id="6a49e-114">1</span><span class="sxs-lookup"><span data-stu-id="6a49e-114">1</span></span>|<span data-ttu-id="6a49e-115">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="6a49e-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="6a49e-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="6a49e-116">highPlus</span></span>|<span data-ttu-id="6a49e-117">duas</span><span class="sxs-lookup"><span data-stu-id="6a49e-117">2</span></span>|<span data-ttu-id="6a49e-118">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="6a49e-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="6a49e-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="6a49e-119">zeroTolerance</span></span>|<span data-ttu-id="6a49e-120">3D</span><span class="sxs-lookup"><span data-stu-id="6a49e-120">3</span></span>|<span data-ttu-id="6a49e-121">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="6a49e-121">Zero tolerance blocks all unknown executables</span></span>|



