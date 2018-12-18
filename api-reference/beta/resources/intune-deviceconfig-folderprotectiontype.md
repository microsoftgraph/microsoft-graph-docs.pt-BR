---
title: tipo de enum folderProtectionType
description: Valores possíveis de proteção de pasta
author: tfitzmac
ms.openlocfilehash: 93df62da9bb5d849cba86b52384f45bfe7bd760f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350600"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="43cac-103">tipo de enum folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="43cac-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="43cac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43cac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43cac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43cac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43cac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43cac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43cac-107">Valores possíveis de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="43cac-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="43cac-108">Membros</span><span class="sxs-lookup"><span data-stu-id="43cac-108">Members</span></span>
|<span data-ttu-id="43cac-109">Membro</span><span class="sxs-lookup"><span data-stu-id="43cac-109">Member</span></span>|<span data-ttu-id="43cac-110">Valor</span><span class="sxs-lookup"><span data-stu-id="43cac-110">Value</span></span>|<span data-ttu-id="43cac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="43cac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cac-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="43cac-112">userDefined</span></span>|<span data-ttu-id="43cac-113">0</span><span class="sxs-lookup"><span data-stu-id="43cac-113">0</span></span>|<span data-ttu-id="43cac-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="43cac-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="43cac-115">Habilitar</span><span class="sxs-lookup"><span data-stu-id="43cac-115">enable</span></span>|<span data-ttu-id="43cac-116">1</span><span class="sxs-lookup"><span data-stu-id="43cac-116">1</span></span>|<span data-ttu-id="43cac-117">Funcionalidade de bloco.</span><span class="sxs-lookup"><span data-stu-id="43cac-117">Block functionality.</span></span>|
|<span data-ttu-id="43cac-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="43cac-118">auditMode</span></span>|<span data-ttu-id="43cac-119">2</span><span class="sxs-lookup"><span data-stu-id="43cac-119">2</span></span>|<span data-ttu-id="43cac-120">Permitir a funcionalidade mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="43cac-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="43cac-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="43cac-121">blockDiskModification</span></span>|<span data-ttu-id="43cac-122">3</span><span class="sxs-lookup"><span data-stu-id="43cac-122">3</span></span>|<span data-ttu-id="43cac-123">Bloquear aplicativos não confiáveis gravem setores do disco.</span><span class="sxs-lookup"><span data-stu-id="43cac-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="43cac-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="43cac-124">auditDiskModification</span></span>|<span data-ttu-id="43cac-125">4</span><span class="sxs-lookup"><span data-stu-id="43cac-125">4</span></span>|<span data-ttu-id="43cac-126">Gere logs quando aplicativos não confiáveis gravar setores do disco.</span><span class="sxs-lookup"><span data-stu-id="43cac-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





