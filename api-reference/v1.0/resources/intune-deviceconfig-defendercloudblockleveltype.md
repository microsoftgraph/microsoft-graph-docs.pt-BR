---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575181"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="aa7a6-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="aa7a6-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="aa7a6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa7a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa7a6-105">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="aa7a6-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="aa7a6-106">Membros</span><span class="sxs-lookup"><span data-stu-id="aa7a6-106">Members</span></span>
|<span data-ttu-id="aa7a6-107">Membro</span><span class="sxs-lookup"><span data-stu-id="aa7a6-107">Member</span></span>|<span data-ttu-id="aa7a6-108">Valor</span><span class="sxs-lookup"><span data-stu-id="aa7a6-108">Value</span></span>|<span data-ttu-id="aa7a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa7a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa7a6-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="aa7a6-110">notConfigured</span></span>|<span data-ttu-id="aa7a6-111">,0</span><span class="sxs-lookup"><span data-stu-id="aa7a6-111">0</span></span>|<span data-ttu-id="aa7a6-112">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="aa7a6-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="aa7a6-113">high</span><span class="sxs-lookup"><span data-stu-id="aa7a6-113">high</span></span>|<span data-ttu-id="aa7a6-114">1 </span><span class="sxs-lookup"><span data-stu-id="aa7a6-114">1</span></span>|<span data-ttu-id="aa7a6-115">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="aa7a6-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="aa7a6-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="aa7a6-116">highPlus</span></span>|<span data-ttu-id="aa7a6-117">2 </span><span class="sxs-lookup"><span data-stu-id="aa7a6-117">2</span></span>|<span data-ttu-id="aa7a6-118">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="aa7a6-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="aa7a6-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="aa7a6-119">zeroTolerance</span></span>|<span data-ttu-id="aa7a6-120">3 </span><span class="sxs-lookup"><span data-stu-id="aa7a6-120">3</span></span>|<span data-ttu-id="aa7a6-121">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="aa7a6-121">Zero tolerance blocks all unknown executables</span></span>|



