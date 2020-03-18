---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a8242f361f68ec7e295950ea29e7478de414ad6b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791734"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="c5cfd-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c5cfd-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="c5cfd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5cfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5cfd-106">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="c5cfd-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="c5cfd-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c5cfd-107">Members</span></span>
|<span data-ttu-id="c5cfd-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c5cfd-108">Member</span></span>|<span data-ttu-id="c5cfd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c5cfd-109">Value</span></span>|<span data-ttu-id="c5cfd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5cfd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5cfd-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="c5cfd-111">userDefined</span></span>|<span data-ttu-id="c5cfd-112">,0</span><span class="sxs-lookup"><span data-stu-id="c5cfd-112">0</span></span>|<span data-ttu-id="c5cfd-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c5cfd-114">possibilite</span><span class="sxs-lookup"><span data-stu-id="c5cfd-114">enable</span></span>|<span data-ttu-id="c5cfd-115">1</span><span class="sxs-lookup"><span data-stu-id="c5cfd-115">1</span></span>|<span data-ttu-id="c5cfd-116">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-116">Block functionality.</span></span>|
|<span data-ttu-id="c5cfd-117">auditmode</span><span class="sxs-lookup"><span data-stu-id="c5cfd-117">auditMode</span></span>|<span data-ttu-id="c5cfd-118">duas</span><span class="sxs-lookup"><span data-stu-id="c5cfd-118">2</span></span>|<span data-ttu-id="c5cfd-119">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="c5cfd-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="c5cfd-120">blockDiskModification</span></span>|<span data-ttu-id="c5cfd-121">3D</span><span class="sxs-lookup"><span data-stu-id="c5cfd-121">3</span></span>|<span data-ttu-id="c5cfd-122">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="c5cfd-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="c5cfd-123">auditDiskModification</span></span>|<span data-ttu-id="c5cfd-124">4 </span><span class="sxs-lookup"><span data-stu-id="c5cfd-124">4</span></span>|<span data-ttu-id="c5cfd-125">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="c5cfd-125">Generate logs when untrusted apps write to disk sectors.</span></span>|



