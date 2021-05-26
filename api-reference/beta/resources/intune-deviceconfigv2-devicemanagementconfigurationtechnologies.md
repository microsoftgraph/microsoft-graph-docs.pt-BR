---
title: tipo de número deviceManagementConfigurationTechnologies
description: Descreve com qual tecnologia essa configuração pode ser implantada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b0e6a6324f9157fb528fd5aeb7772f4c1e8721fe
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666692"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a><span data-ttu-id="ea4b5-103">tipo de número deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="ea4b5-103">deviceManagementConfigurationTechnologies enum type</span></span>

<span data-ttu-id="ea4b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea4b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea4b5-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea4b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea4b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea4b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea4b5-107">Descreve com qual tecnologia essa configuração pode ser implantada</span><span class="sxs-lookup"><span data-stu-id="ea4b5-107">Describes which technology this setting can be deployed with</span></span>

## <a name="members"></a><span data-ttu-id="ea4b5-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ea4b5-108">Members</span></span>
|<span data-ttu-id="ea4b5-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ea4b5-109">Member</span></span>|<span data-ttu-id="ea4b5-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ea4b5-110">Value</span></span>|<span data-ttu-id="ea4b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4b5-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="ea4b5-112">none</span></span>|<span data-ttu-id="ea4b5-113">0</span><span class="sxs-lookup"><span data-stu-id="ea4b5-113">0</span></span>|<span data-ttu-id="ea4b5-114">A configuração não pode ser implantada por meio de qualquer canal</span><span class="sxs-lookup"><span data-stu-id="ea4b5-114">Setting cannot be deployed through any channel</span></span>|
|<span data-ttu-id="ea4b5-115">mdm</span><span class="sxs-lookup"><span data-stu-id="ea4b5-115">mdm</span></span>|<span data-ttu-id="ea4b5-116">1</span><span class="sxs-lookup"><span data-stu-id="ea4b5-116">1</span></span>|<span data-ttu-id="ea4b5-117">A configuração pode ser implantada por meio do canal MDM</span><span class="sxs-lookup"><span data-stu-id="ea4b5-117">Setting can be deployed through the MDM channel</span></span>|
|<span data-ttu-id="ea4b5-118">windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="ea4b5-118">windows10XManagement</span></span>|<span data-ttu-id="ea4b5-119">2</span><span class="sxs-lookup"><span data-stu-id="ea4b5-119">2</span></span>|<span data-ttu-id="ea4b5-120">A configuração pode ser implantada por meio do canal Windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="ea4b5-120">Setting can be deployed through the Windows10XManagement channel</span></span>|
|<span data-ttu-id="ea4b5-121">configManager</span><span class="sxs-lookup"><span data-stu-id="ea4b5-121">configManager</span></span>|<span data-ttu-id="ea4b5-122">4 </span><span class="sxs-lookup"><span data-stu-id="ea4b5-122">4</span></span>|<span data-ttu-id="ea4b5-123">A configuração pode ser implantada por meio do canal ConfigManager</span><span class="sxs-lookup"><span data-stu-id="ea4b5-123">Setting can be deployed through the ConfigManager channel</span></span>|
|<span data-ttu-id="ea4b5-124">microsoftSense</span><span class="sxs-lookup"><span data-stu-id="ea4b5-124">microsoftSense</span></span>|<span data-ttu-id="ea4b5-125">128</span><span class="sxs-lookup"><span data-stu-id="ea4b5-125">128</span></span>|<span data-ttu-id="ea4b5-126">A configuração pode ser implantada por meio do canal do agente SENSE</span><span class="sxs-lookup"><span data-stu-id="ea4b5-126">Setting can be deployed through the SENSE agent channel</span></span>|




