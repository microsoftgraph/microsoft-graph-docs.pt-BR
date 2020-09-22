---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8fd63865369371a32a1bda0b2a7438fc851256a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069019"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="0dd13-103">tipo de enumeração defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="0dd13-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="0dd13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dd13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dd13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dd13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dd13-106">Possíveis valores de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="0dd13-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="0dd13-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0dd13-107">Members</span></span>
|<span data-ttu-id="0dd13-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0dd13-108">Member</span></span>|<span data-ttu-id="0dd13-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0dd13-109">Value</span></span>|<span data-ttu-id="0dd13-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dd13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd13-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0dd13-111">notConfigured</span></span>|<span data-ttu-id="0dd13-112">,0</span><span class="sxs-lookup"><span data-stu-id="0dd13-112">0</span></span>|<span data-ttu-id="0dd13-113">O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="0dd13-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="0dd13-114">high</span><span class="sxs-lookup"><span data-stu-id="0dd13-114">high</span></span>|<span data-ttu-id="0dd13-115">1 </span><span class="sxs-lookup"><span data-stu-id="0dd13-115">1</span></span>|<span data-ttu-id="0dd13-116">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="0dd13-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="0dd13-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="0dd13-117">highPlus</span></span>|<span data-ttu-id="0dd13-118">2 </span><span class="sxs-lookup"><span data-stu-id="0dd13-118">2</span></span>|<span data-ttu-id="0dd13-119">High + usa o alto nível e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="0dd13-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="0dd13-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="0dd13-120">zeroTolerance</span></span>|<span data-ttu-id="0dd13-121">3D</span><span class="sxs-lookup"><span data-stu-id="0dd13-121">3</span></span>|<span data-ttu-id="0dd13-122">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="0dd13-122">Zero tolerance blocks all unknown executables</span></span>|









