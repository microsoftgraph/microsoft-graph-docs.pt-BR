---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 61c41f8e2d9d0b787988a10e0562d10567bf1b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071049"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="165ec-103">tipo de enumeração win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="165ec-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="165ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="165ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="165ec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="165ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="165ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="165ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="165ec-107">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="165ec-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="165ec-108">Membros</span><span class="sxs-lookup"><span data-stu-id="165ec-108">Members</span></span>
|<span data-ttu-id="165ec-109">Membro</span><span class="sxs-lookup"><span data-stu-id="165ec-109">Member</span></span>|<span data-ttu-id="165ec-110">Valor</span><span class="sxs-lookup"><span data-stu-id="165ec-110">Value</span></span>|<span data-ttu-id="165ec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="165ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165ec-112">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="165ec-112">basedOnReturnCode</span></span>|<span data-ttu-id="165ec-113">,0</span><span class="sxs-lookup"><span data-stu-id="165ec-113">0</span></span>|<span data-ttu-id="165ec-114">O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="165ec-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="165ec-115">permitiu</span><span class="sxs-lookup"><span data-stu-id="165ec-115">allow</span></span>|<span data-ttu-id="165ec-116">1 </span><span class="sxs-lookup"><span data-stu-id="165ec-116">1</span></span>|<span data-ttu-id="165ec-117">O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="165ec-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="165ec-118">O Intune não tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="165ec-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="165ec-119">eliminação</span><span class="sxs-lookup"><span data-stu-id="165ec-119">suppress</span></span>|<span data-ttu-id="165ec-120">2 </span><span class="sxs-lookup"><span data-stu-id="165ec-120">2</span></span>|<span data-ttu-id="165ec-121">O Intune tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="165ec-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="165ec-122">vigor</span><span class="sxs-lookup"><span data-stu-id="165ec-122">force</span></span>|<span data-ttu-id="165ec-123">3 </span><span class="sxs-lookup"><span data-stu-id="165ec-123">3</span></span>|<span data-ttu-id="165ec-124">O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="165ec-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|






