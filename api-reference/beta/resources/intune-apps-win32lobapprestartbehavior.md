---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2902f3808ea1ebcc1442b0675c89da51b059f2c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422636"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="d85c8-103">tipo de enumeração win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="d85c8-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="d85c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d85c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d85c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d85c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d85c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d85c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d85c8-107">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d85c8-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="d85c8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d85c8-108">Members</span></span>
|<span data-ttu-id="d85c8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d85c8-109">Member</span></span>|<span data-ttu-id="d85c8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d85c8-110">Value</span></span>|<span data-ttu-id="d85c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d85c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d85c8-112">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="d85c8-112">basedOnReturnCode</span></span>|<span data-ttu-id="d85c8-113">,0</span><span class="sxs-lookup"><span data-stu-id="d85c8-113">0</span></span>|<span data-ttu-id="d85c8-114">O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d85c8-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="d85c8-115">permitiu</span><span class="sxs-lookup"><span data-stu-id="d85c8-115">allow</span></span>|<span data-ttu-id="d85c8-116">1</span><span class="sxs-lookup"><span data-stu-id="d85c8-116">1</span></span>|<span data-ttu-id="d85c8-117">O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d85c8-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="d85c8-118">O Intune não tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="d85c8-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="d85c8-119">eliminação</span><span class="sxs-lookup"><span data-stu-id="d85c8-119">suppress</span></span>|<span data-ttu-id="d85c8-120">duas</span><span class="sxs-lookup"><span data-stu-id="d85c8-120">2</span></span>|<span data-ttu-id="d85c8-121">O Intune tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="d85c8-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="d85c8-122">vigor</span><span class="sxs-lookup"><span data-stu-id="d85c8-122">force</span></span>|<span data-ttu-id="d85c8-123">3D</span><span class="sxs-lookup"><span data-stu-id="d85c8-123">3</span></span>|<span data-ttu-id="d85c8-124">O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d85c8-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|



