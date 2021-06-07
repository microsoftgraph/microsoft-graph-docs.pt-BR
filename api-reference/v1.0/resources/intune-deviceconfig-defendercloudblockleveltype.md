---
title: Tipo denum defenderCloudBlockLevelType
description: Valores possíveis do Nível de Bloqueio na Nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755886"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f0d94-103">Tipo denum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="f0d94-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="f0d94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0d94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0d94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0d94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0d94-106">Valores possíveis do Nível de Bloqueio na Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d94-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="f0d94-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f0d94-107">Members</span></span>
|<span data-ttu-id="f0d94-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f0d94-108">Member</span></span>|<span data-ttu-id="f0d94-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f0d94-109">Value</span></span>|<span data-ttu-id="f0d94-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0d94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0d94-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f0d94-111">notConfigured</span></span>|<span data-ttu-id="f0d94-112">0</span><span class="sxs-lookup"><span data-stu-id="f0d94-112">0</span></span>|<span data-ttu-id="f0d94-113">Valor padrão, usa o nível de bloqueio padrão Windows Defender Antivírus e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="f0d94-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f0d94-114">high</span><span class="sxs-lookup"><span data-stu-id="f0d94-114">high</span></span>|<span data-ttu-id="f0d94-115">1</span><span class="sxs-lookup"><span data-stu-id="f0d94-115">1</span></span>|<span data-ttu-id="f0d94-116">Alto aplica um nível forte de detecção.</span><span class="sxs-lookup"><span data-stu-id="f0d94-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f0d94-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="f0d94-117">highPlus</span></span>|<span data-ttu-id="f0d94-118">2</span><span class="sxs-lookup"><span data-stu-id="f0d94-118">2</span></span>|<span data-ttu-id="f0d94-119">High + usa o nível Alto e aplica medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="f0d94-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f0d94-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="f0d94-120">zeroTolerance</span></span>|<span data-ttu-id="f0d94-121">3</span><span class="sxs-lookup"><span data-stu-id="f0d94-121">3</span></span>|<span data-ttu-id="f0d94-122">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f0d94-122">Zero tolerance blocks all unknown executables</span></span>|




