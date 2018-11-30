---
title: tipo de enum folderProtectionType
description: Valores possíveis de proteção de pasta
ms.openlocfilehash: a02f1602f8b9a962124fb7bf2a9731662a6f3057
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036018"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="6a914-103">tipo de enum folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6a914-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="6a914-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a914-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a914-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a914-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a914-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a914-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a914-107">Valores possíveis de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="6a914-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="6a914-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6a914-108">Members</span></span>
|<span data-ttu-id="6a914-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6a914-109">Member</span></span>|<span data-ttu-id="6a914-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6a914-110">Value</span></span>|<span data-ttu-id="6a914-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a914-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a914-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="6a914-112">userDefined</span></span>|<span data-ttu-id="6a914-113">0</span><span class="sxs-lookup"><span data-stu-id="6a914-113">0</span></span>|<span data-ttu-id="6a914-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6a914-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6a914-115">Habilitar</span><span class="sxs-lookup"><span data-stu-id="6a914-115">enable</span></span>|<span data-ttu-id="6a914-116">1</span><span class="sxs-lookup"><span data-stu-id="6a914-116">1</span></span>|<span data-ttu-id="6a914-117">Funcionalidade de bloco.</span><span class="sxs-lookup"><span data-stu-id="6a914-117">Block functionality.</span></span>|
|<span data-ttu-id="6a914-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="6a914-118">auditMode</span></span>|<span data-ttu-id="6a914-119">2</span><span class="sxs-lookup"><span data-stu-id="6a914-119">2</span></span>|<span data-ttu-id="6a914-120">Permitir a funcionalidade mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="6a914-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="6a914-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="6a914-121">blockDiskModification</span></span>|<span data-ttu-id="6a914-122">3</span><span class="sxs-lookup"><span data-stu-id="6a914-122">3</span></span>|<span data-ttu-id="6a914-123">Bloquear aplicativos não confiáveis gravem setores do disco.</span><span class="sxs-lookup"><span data-stu-id="6a914-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="6a914-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="6a914-124">auditDiskModification</span></span>|<span data-ttu-id="6a914-125">4</span><span class="sxs-lookup"><span data-stu-id="6a914-125">4</span></span>|<span data-ttu-id="6a914-126">Gere logs quando aplicativos não confiáveis gravar setores do disco.</span><span class="sxs-lookup"><span data-stu-id="6a914-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





