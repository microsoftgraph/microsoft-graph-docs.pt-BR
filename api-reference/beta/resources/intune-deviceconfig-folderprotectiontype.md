---
title: tipo de enumeração folderProtectionType
description: Possíveis valores de proteção de pasta
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 23717d1e798059f1ca025a3f80279804b616b17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529983"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="4f7a0-103">tipo de enumeração folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4f7a0-103">folderProtectionType enum type</span></span>

<span data-ttu-id="4f7a0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f7a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f7a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f7a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f7a0-107">Possíveis valores de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="4f7a0-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="4f7a0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4f7a0-108">Members</span></span>
|<span data-ttu-id="4f7a0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4f7a0-109">Member</span></span>|<span data-ttu-id="4f7a0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4f7a0-110">Value</span></span>|<span data-ttu-id="4f7a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f7a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f7a0-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="4f7a0-112">userDefined</span></span>|<span data-ttu-id="4f7a0-113">,0</span><span class="sxs-lookup"><span data-stu-id="4f7a0-113">0</span></span>|<span data-ttu-id="4f7a0-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="4f7a0-115">possibilite</span><span class="sxs-lookup"><span data-stu-id="4f7a0-115">enable</span></span>|<span data-ttu-id="4f7a0-116">1 </span><span class="sxs-lookup"><span data-stu-id="4f7a0-116">1</span></span>|<span data-ttu-id="4f7a0-117">Funcionalidade de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-117">Block functionality.</span></span>|
|<span data-ttu-id="4f7a0-118">auditmode</span><span class="sxs-lookup"><span data-stu-id="4f7a0-118">auditMode</span></span>|<span data-ttu-id="4f7a0-119">2 </span><span class="sxs-lookup"><span data-stu-id="4f7a0-119">2</span></span>|<span data-ttu-id="4f7a0-120">Permitir a funcionalidade, mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="4f7a0-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="4f7a0-121">blockDiskModification</span></span>|<span data-ttu-id="4f7a0-122">3 </span><span class="sxs-lookup"><span data-stu-id="4f7a0-122">3</span></span>|<span data-ttu-id="4f7a0-123">Bloquear a gravação de aplicativos não confiáveis em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="4f7a0-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="4f7a0-124">auditDiskModification</span></span>|<span data-ttu-id="4f7a0-125">4 </span><span class="sxs-lookup"><span data-stu-id="4f7a0-125">4</span></span>|<span data-ttu-id="4f7a0-126">Gerar logs quando aplicativos não confiáveis gravam em setores de disco.</span><span class="sxs-lookup"><span data-stu-id="4f7a0-126">Generate logs when untrusted apps write to disk sectors.</span></span>|



