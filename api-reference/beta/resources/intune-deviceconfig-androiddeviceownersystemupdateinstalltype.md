---
title: tipo de enumeração androidDeviceOwnerSystemUpdateInstallType
description: Tipos de atualização do sistema para o proprietário do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3d5c9ba006bd155f2452242feadc5d965bf6d451
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486098"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="568a6-103">tipo de enumeração androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="568a6-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

<span data-ttu-id="568a6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="568a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="568a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="568a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="568a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="568a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568a6-107">Tipos de atualização do sistema para o proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="568a6-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="568a6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="568a6-108">Members</span></span>
|<span data-ttu-id="568a6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="568a6-109">Member</span></span>|<span data-ttu-id="568a6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="568a6-110">Value</span></span>|<span data-ttu-id="568a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="568a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="568a6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="568a6-112">deviceDefault</span></span>|<span data-ttu-id="568a6-113">,0</span><span class="sxs-lookup"><span data-stu-id="568a6-113">0</span></span>|<span data-ttu-id="568a6-114">Comportamento padrão do dispositivo, que normalmente solicita que o usuário aceite atualizações do sistema.</span><span class="sxs-lookup"><span data-stu-id="568a6-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="568a6-115">adiamento</span><span class="sxs-lookup"><span data-stu-id="568a6-115">postpone</span></span>|<span data-ttu-id="568a6-116">1 </span><span class="sxs-lookup"><span data-stu-id="568a6-116">1</span></span>|<span data-ttu-id="568a6-117">Adiar a instalação automática de atualizações até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="568a6-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="568a6-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="568a6-118">windowed</span></span>|<span data-ttu-id="568a6-119">2 </span><span class="sxs-lookup"><span data-stu-id="568a6-119">2</span></span>|<span data-ttu-id="568a6-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="568a6-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="568a6-121">Automático</span><span class="sxs-lookup"><span data-stu-id="568a6-121">automatic</span></span>|<span data-ttu-id="568a6-122">3 </span><span class="sxs-lookup"><span data-stu-id="568a6-122">3</span></span>|<span data-ttu-id="568a6-123">Instalar atualizações automaticamente o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="568a6-123">Automatically install updates as soon as possible.</span></span>|



