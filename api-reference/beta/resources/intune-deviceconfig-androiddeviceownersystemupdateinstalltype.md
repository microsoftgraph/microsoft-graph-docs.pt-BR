---
title: tipo de enum androidDeviceOwnerSystemUpdateInstallType
description: Atualizar tipos de sistema para o proprietário de dispositivo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a46d60972bab46fa0e2cda8d03a090bd8b810a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980969"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="1e73d-103">tipo de enum androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1e73d-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="1e73d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e73d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e73d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e73d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e73d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e73d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e73d-107">Atualizar tipos de sistema para o proprietário de dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="1e73d-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="1e73d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1e73d-108">Members</span></span>
|<span data-ttu-id="1e73d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1e73d-109">Member</span></span>|<span data-ttu-id="1e73d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1e73d-110">Value</span></span>|<span data-ttu-id="1e73d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e73d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e73d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1e73d-112">deviceDefault</span></span>|<span data-ttu-id="1e73d-113">0</span><span class="sxs-lookup"><span data-stu-id="1e73d-113">0</span></span>|<span data-ttu-id="1e73d-114">Comportamento de padrão de dispositivo, que geralmente solicita que o usuário aceite atualizações de sistema.</span><span class="sxs-lookup"><span data-stu-id="1e73d-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="1e73d-115">Adiar</span><span class="sxs-lookup"><span data-stu-id="1e73d-115">postpone</span></span>|<span data-ttu-id="1e73d-116">1</span><span class="sxs-lookup"><span data-stu-id="1e73d-116">1</span></span>|<span data-ttu-id="1e73d-117">Adie a instalação automática das atualizações de backup para 30 dias.</span><span class="sxs-lookup"><span data-stu-id="1e73d-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="1e73d-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="1e73d-118">windowed</span></span>|<span data-ttu-id="1e73d-119">2</span><span class="sxs-lookup"><span data-stu-id="1e73d-119">2</span></span>|<span data-ttu-id="1e73d-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="1e73d-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="1e73d-121">automatic</span><span class="sxs-lookup"><span data-stu-id="1e73d-121">automatic</span></span>|<span data-ttu-id="1e73d-122">3</span><span class="sxs-lookup"><span data-stu-id="1e73d-122">3</span></span>|<span data-ttu-id="1e73d-123">Instale automaticamente atualizações assim que possível.</span><span class="sxs-lookup"><span data-stu-id="1e73d-123">Automatically install updates as soon as possible.</span></span>|





