---
title: tipo de enum folderProtectionType
description: Valores possíveis de proteção de pasta
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405713"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="ac35b-103">tipo de enum folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ac35b-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="ac35b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac35b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac35b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac35b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac35b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ac35b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac35b-107">Valores possíveis de proteção de pasta</span><span class="sxs-lookup"><span data-stu-id="ac35b-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="ac35b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ac35b-108">Members</span></span>
|<span data-ttu-id="ac35b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ac35b-109">Member</span></span>|<span data-ttu-id="ac35b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ac35b-110">Value</span></span>|<span data-ttu-id="ac35b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac35b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac35b-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="ac35b-112">userDefined</span></span>|<span data-ttu-id="ac35b-113">0</span><span class="sxs-lookup"><span data-stu-id="ac35b-113">0</span></span>|<span data-ttu-id="ac35b-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="ac35b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="ac35b-115">Habilitar</span><span class="sxs-lookup"><span data-stu-id="ac35b-115">enable</span></span>|<span data-ttu-id="ac35b-116">1</span><span class="sxs-lookup"><span data-stu-id="ac35b-116">1</span></span>|<span data-ttu-id="ac35b-117">Funcionalidade de bloco.</span><span class="sxs-lookup"><span data-stu-id="ac35b-117">Block functionality.</span></span>|
|<span data-ttu-id="ac35b-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="ac35b-118">auditMode</span></span>|<span data-ttu-id="ac35b-119">2</span><span class="sxs-lookup"><span data-stu-id="ac35b-119">2</span></span>|<span data-ttu-id="ac35b-120">Permitir a funcionalidade mas gerar logs.</span><span class="sxs-lookup"><span data-stu-id="ac35b-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="ac35b-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="ac35b-121">blockDiskModification</span></span>|<span data-ttu-id="ac35b-122">3</span><span class="sxs-lookup"><span data-stu-id="ac35b-122">3</span></span>|<span data-ttu-id="ac35b-123">Bloquear aplicativos não confiáveis gravem setores do disco.</span><span class="sxs-lookup"><span data-stu-id="ac35b-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="ac35b-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="ac35b-124">auditDiskModification</span></span>|<span data-ttu-id="ac35b-125">4</span><span class="sxs-lookup"><span data-stu-id="ac35b-125">4</span></span>|<span data-ttu-id="ac35b-126">Gere logs quando aplicativos não confiáveis gravar setores do disco.</span><span class="sxs-lookup"><span data-stu-id="ac35b-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




