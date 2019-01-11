---
title: tipo de enum folderProtectionType
description: Valores possíveis de proteção de pasta
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 435f3ea01f5a8ffc3c4cb54034d415d54732db5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826128"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="a7a60-103">tipo de enum folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7a60-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="a7a60-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7a60-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7a60-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7a60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7a60-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7a60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7a60-107">Valores possíveis de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="a7a60-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="a7a60-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a7a60-108">Members</span></span>
|<span data-ttu-id="a7a60-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a7a60-109">Member</span></span>|<span data-ttu-id="a7a60-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a7a60-110">Value</span></span>|<span data-ttu-id="a7a60-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7a60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a60-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="a7a60-112">userDefined</span></span>|<span data-ttu-id="a7a60-113">0</span><span class="sxs-lookup"><span data-stu-id="a7a60-113">0</span></span>|<span data-ttu-id="a7a60-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a7a60-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a7a60-115">Habilitar</span><span class="sxs-lookup"><span data-stu-id="a7a60-115">enable</span></span>|<span data-ttu-id="a7a60-116">1</span><span class="sxs-lookup"><span data-stu-id="a7a60-116">1</span></span>|<span data-ttu-id="a7a60-117">Funcionalidade de bloco.</span><span class="sxs-lookup"><span data-stu-id="a7a60-117">Block functionality.</span></span>|
|<span data-ttu-id="a7a60-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="a7a60-118">auditMode</span></span>|<span data-ttu-id="a7a60-119">2</span><span class="sxs-lookup"><span data-stu-id="a7a60-119">2</span></span>|<span data-ttu-id="a7a60-120">Permitir a funcionalidade mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="a7a60-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="a7a60-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="a7a60-121">blockDiskModification</span></span>|<span data-ttu-id="a7a60-122">3</span><span class="sxs-lookup"><span data-stu-id="a7a60-122">3</span></span>|<span data-ttu-id="a7a60-123">Bloquear aplicativos não confiáveis gravem setores do disco.</span><span class="sxs-lookup"><span data-stu-id="a7a60-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="a7a60-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="a7a60-124">auditDiskModification</span></span>|<span data-ttu-id="a7a60-125">4</span><span class="sxs-lookup"><span data-stu-id="a7a60-125">4</span></span>|<span data-ttu-id="a7a60-126">Gere logs quando aplicativos não confiáveis gravar setores do disco.</span><span class="sxs-lookup"><span data-stu-id="a7a60-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





