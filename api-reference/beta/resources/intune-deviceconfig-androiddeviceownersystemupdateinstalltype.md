---
title: tipo de enumeração androidDeviceOwnerSystemUpdateInstallType
description: Tipos de atualização do sistema para o proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 06f0f91410f12f6bff8a7e3c427e248423324079
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073933"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="9508d-103">tipo de enumeração androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="9508d-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

<span data-ttu-id="9508d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9508d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9508d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9508d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9508d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9508d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9508d-107">Tipos de atualização do sistema para o proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="9508d-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="9508d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9508d-108">Members</span></span>
|<span data-ttu-id="9508d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9508d-109">Member</span></span>|<span data-ttu-id="9508d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9508d-110">Value</span></span>|<span data-ttu-id="9508d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9508d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9508d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9508d-112">deviceDefault</span></span>|<span data-ttu-id="9508d-113">,0</span><span class="sxs-lookup"><span data-stu-id="9508d-113">0</span></span>|<span data-ttu-id="9508d-114">Comportamento padrão do dispositivo, que normalmente solicita que o usuário aceite atualizações do sistema.</span><span class="sxs-lookup"><span data-stu-id="9508d-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="9508d-115">adiamento</span><span class="sxs-lookup"><span data-stu-id="9508d-115">postpone</span></span>|<span data-ttu-id="9508d-116">1 </span><span class="sxs-lookup"><span data-stu-id="9508d-116">1</span></span>|<span data-ttu-id="9508d-117">Adiar a instalação automática de atualizações até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="9508d-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="9508d-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="9508d-118">windowed</span></span>|<span data-ttu-id="9508d-119">2 </span><span class="sxs-lookup"><span data-stu-id="9508d-119">2</span></span>|<span data-ttu-id="9508d-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="9508d-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="9508d-121">Automático</span><span class="sxs-lookup"><span data-stu-id="9508d-121">automatic</span></span>|<span data-ttu-id="9508d-122">3 </span><span class="sxs-lookup"><span data-stu-id="9508d-122">3</span></span>|<span data-ttu-id="9508d-123">Instalar atualizações automaticamente o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="9508d-123">Automatically install updates as soon as possible.</span></span>|






