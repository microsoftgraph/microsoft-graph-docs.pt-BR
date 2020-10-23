---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc508f3feaf1353d83a87cd0403f9ede2bbcad13
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730483"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="66d01-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66d01-103">folderProtectionType enum type</span></span>

<span data-ttu-id="66d01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66d01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66d01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66d01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d01-107">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="66d01-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="66d01-108">Membros</span><span class="sxs-lookup"><span data-stu-id="66d01-108">Members</span></span>
|<span data-ttu-id="66d01-109">Membro</span><span class="sxs-lookup"><span data-stu-id="66d01-109">Member</span></span>|<span data-ttu-id="66d01-110">Valor</span><span class="sxs-lookup"><span data-stu-id="66d01-110">Value</span></span>|<span data-ttu-id="66d01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d01-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="66d01-112">userDefined</span></span>|<span data-ttu-id="66d01-113">,0</span><span class="sxs-lookup"><span data-stu-id="66d01-113">0</span></span>|<span data-ttu-id="66d01-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="66d01-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="66d01-115">possibilite</span><span class="sxs-lookup"><span data-stu-id="66d01-115">enable</span></span>|<span data-ttu-id="66d01-116">1</span><span class="sxs-lookup"><span data-stu-id="66d01-116">1</span></span>|<span data-ttu-id="66d01-117">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="66d01-117">Block functionality.</span></span>|
|<span data-ttu-id="66d01-118">auditmode</span><span class="sxs-lookup"><span data-stu-id="66d01-118">auditMode</span></span>|<span data-ttu-id="66d01-119">duas</span><span class="sxs-lookup"><span data-stu-id="66d01-119">2</span></span>|<span data-ttu-id="66d01-120">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="66d01-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="66d01-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="66d01-121">blockDiskModification</span></span>|<span data-ttu-id="66d01-122">3D</span><span class="sxs-lookup"><span data-stu-id="66d01-122">3</span></span>|<span data-ttu-id="66d01-123">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="66d01-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="66d01-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="66d01-124">auditDiskModification</span></span>|<span data-ttu-id="66d01-125">4 </span><span class="sxs-lookup"><span data-stu-id="66d01-125">4</span></span>|<span data-ttu-id="66d01-126">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="66d01-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





