---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ccdaf6625685a0e9e317ad01c8b81fffa04f651
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994068"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="e7944-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e7944-103">folderProtectionType enum type</span></span>

<span data-ttu-id="e7944-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7944-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7944-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7944-107">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="e7944-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="e7944-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e7944-108">Members</span></span>
|<span data-ttu-id="e7944-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e7944-109">Member</span></span>|<span data-ttu-id="e7944-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e7944-110">Value</span></span>|<span data-ttu-id="e7944-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7944-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7944-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="e7944-112">userDefined</span></span>|<span data-ttu-id="e7944-113">,0</span><span class="sxs-lookup"><span data-stu-id="e7944-113">0</span></span>|<span data-ttu-id="e7944-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="e7944-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e7944-115">possibilite</span><span class="sxs-lookup"><span data-stu-id="e7944-115">enable</span></span>|<span data-ttu-id="e7944-116">1 </span><span class="sxs-lookup"><span data-stu-id="e7944-116">1</span></span>|<span data-ttu-id="e7944-117">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="e7944-117">Block functionality.</span></span>|
|<span data-ttu-id="e7944-118">auditmode</span><span class="sxs-lookup"><span data-stu-id="e7944-118">auditMode</span></span>|<span data-ttu-id="e7944-119">2 </span><span class="sxs-lookup"><span data-stu-id="e7944-119">2</span></span>|<span data-ttu-id="e7944-120">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="e7944-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="e7944-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="e7944-121">blockDiskModification</span></span>|<span data-ttu-id="e7944-122">3 </span><span class="sxs-lookup"><span data-stu-id="e7944-122">3</span></span>|<span data-ttu-id="e7944-123">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="e7944-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="e7944-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="e7944-124">auditDiskModification</span></span>|<span data-ttu-id="e7944-125">4 </span><span class="sxs-lookup"><span data-stu-id="e7944-125">4</span></span>|<span data-ttu-id="e7944-126">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="e7944-126">Generate logs when untrusted apps write to disk sectors.</span></span>|






