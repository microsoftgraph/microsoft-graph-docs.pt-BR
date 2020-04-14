---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ded583dfe44d393a2ae1c8f56f9952feb85cf857
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444285"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="fcd18-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="fcd18-103">folderProtectionType enum type</span></span>

<span data-ttu-id="fcd18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcd18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcd18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fcd18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcd18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcd18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcd18-107">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="fcd18-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="fcd18-108">Membros</span><span class="sxs-lookup"><span data-stu-id="fcd18-108">Members</span></span>
|<span data-ttu-id="fcd18-109">Membro</span><span class="sxs-lookup"><span data-stu-id="fcd18-109">Member</span></span>|<span data-ttu-id="fcd18-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fcd18-110">Value</span></span>|<span data-ttu-id="fcd18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcd18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcd18-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="fcd18-112">userDefined</span></span>|<span data-ttu-id="fcd18-113">,0</span><span class="sxs-lookup"><span data-stu-id="fcd18-113">0</span></span>|<span data-ttu-id="fcd18-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="fcd18-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="fcd18-115">possibilite</span><span class="sxs-lookup"><span data-stu-id="fcd18-115">enable</span></span>|<span data-ttu-id="fcd18-116">1</span><span class="sxs-lookup"><span data-stu-id="fcd18-116">1</span></span>|<span data-ttu-id="fcd18-117">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="fcd18-117">Block functionality.</span></span>|
|<span data-ttu-id="fcd18-118">auditmode</span><span class="sxs-lookup"><span data-stu-id="fcd18-118">auditMode</span></span>|<span data-ttu-id="fcd18-119">duas</span><span class="sxs-lookup"><span data-stu-id="fcd18-119">2</span></span>|<span data-ttu-id="fcd18-120">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="fcd18-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="fcd18-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="fcd18-121">blockDiskModification</span></span>|<span data-ttu-id="fcd18-122">3D</span><span class="sxs-lookup"><span data-stu-id="fcd18-122">3</span></span>|<span data-ttu-id="fcd18-123">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="fcd18-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="fcd18-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="fcd18-124">auditDiskModification</span></span>|<span data-ttu-id="fcd18-125">4 </span><span class="sxs-lookup"><span data-stu-id="fcd18-125">4</span></span>|<span data-ttu-id="fcd18-126">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="fcd18-126">Generate logs when untrusted apps write to disk sectors.</span></span>|



