---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 16fda1d530614ea138ecc575930b4800b5f143c4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797553"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="b9864-103">tipo de enumeração win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="b9864-103">win32LobAppRestartBehavior enum type</span></span>

> <span data-ttu-id="b9864-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9864-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9864-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9864-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9864-106">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="b9864-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="b9864-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b9864-107">Members</span></span>
|<span data-ttu-id="b9864-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b9864-108">Member</span></span>|<span data-ttu-id="b9864-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b9864-109">Value</span></span>|<span data-ttu-id="b9864-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9864-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9864-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="b9864-111">basedOnReturnCode</span></span>|<span data-ttu-id="b9864-112">,0</span><span class="sxs-lookup"><span data-stu-id="b9864-112">0</span></span>|<span data-ttu-id="b9864-113">O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="b9864-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="b9864-114">permitiu</span><span class="sxs-lookup"><span data-stu-id="b9864-114">allow</span></span>|<span data-ttu-id="b9864-115">1</span><span class="sxs-lookup"><span data-stu-id="b9864-115">1</span></span>|<span data-ttu-id="b9864-116">O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b9864-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="b9864-117">O Intune não tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="b9864-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b9864-118">eliminação</span><span class="sxs-lookup"><span data-stu-id="b9864-118">suppress</span></span>|<span data-ttu-id="b9864-119">duas</span><span class="sxs-lookup"><span data-stu-id="b9864-119">2</span></span>|<span data-ttu-id="b9864-120">O Intune tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="b9864-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b9864-121">vigor</span><span class="sxs-lookup"><span data-stu-id="b9864-121">force</span></span>|<span data-ttu-id="b9864-122">3D</span><span class="sxs-lookup"><span data-stu-id="b9864-122">3</span></span>|<span data-ttu-id="b9864-123">O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9864-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|



