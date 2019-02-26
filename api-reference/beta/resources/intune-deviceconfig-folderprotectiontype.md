---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170333"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="31fac-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="31fac-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="31fac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31fac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31fac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31fac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31fac-106">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="31fac-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="31fac-107">Membros</span><span class="sxs-lookup"><span data-stu-id="31fac-107">Members</span></span>
|<span data-ttu-id="31fac-108">Membro</span><span class="sxs-lookup"><span data-stu-id="31fac-108">Member</span></span>|<span data-ttu-id="31fac-109">Valor</span><span class="sxs-lookup"><span data-stu-id="31fac-109">Value</span></span>|<span data-ttu-id="31fac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="31fac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31fac-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="31fac-111">userDefined</span></span>|<span data-ttu-id="31fac-112">,0</span><span class="sxs-lookup"><span data-stu-id="31fac-112">0</span></span>|<span data-ttu-id="31fac-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="31fac-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="31fac-114">possibilite</span><span class="sxs-lookup"><span data-stu-id="31fac-114">enable</span></span>|<span data-ttu-id="31fac-115">1</span><span class="sxs-lookup"><span data-stu-id="31fac-115">1</span></span>|<span data-ttu-id="31fac-116">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="31fac-116">Block functionality.</span></span>|
|<span data-ttu-id="31fac-117">auditmode</span><span class="sxs-lookup"><span data-stu-id="31fac-117">auditMode</span></span>|<span data-ttu-id="31fac-118">duas</span><span class="sxs-lookup"><span data-stu-id="31fac-118">2</span></span>|<span data-ttu-id="31fac-119">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="31fac-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="31fac-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="31fac-120">blockDiskModification</span></span>|<span data-ttu-id="31fac-121">3D</span><span class="sxs-lookup"><span data-stu-id="31fac-121">3</span></span>|<span data-ttu-id="31fac-122">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="31fac-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="31fac-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="31fac-123">auditDiskModification</span></span>|<span data-ttu-id="31fac-124">quatro</span><span class="sxs-lookup"><span data-stu-id="31fac-124">4</span></span>|<span data-ttu-id="31fac-125">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="31fac-125">Generate logs when untrusted apps write to disk sectors.</span></span>|




