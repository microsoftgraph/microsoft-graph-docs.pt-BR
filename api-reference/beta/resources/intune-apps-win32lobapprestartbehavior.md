---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6747b9b0b3f46e5c2fcf913725d915232a1559ed
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538543"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="dc786-103">tipo de enumeração win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="dc786-103">win32LobAppRestartBehavior enum type</span></span>

> <span data-ttu-id="dc786-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc786-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc786-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc786-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc786-106">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="dc786-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="dc786-107">Membros</span><span class="sxs-lookup"><span data-stu-id="dc786-107">Members</span></span>
|<span data-ttu-id="dc786-108">Membro</span><span class="sxs-lookup"><span data-stu-id="dc786-108">Member</span></span>|<span data-ttu-id="dc786-109">Valor</span><span class="sxs-lookup"><span data-stu-id="dc786-109">Value</span></span>|<span data-ttu-id="dc786-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc786-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc786-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="dc786-111">basedOnReturnCode</span></span>|<span data-ttu-id="dc786-112">,0</span><span class="sxs-lookup"><span data-stu-id="dc786-112">0</span></span>|<span data-ttu-id="dc786-113">O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="dc786-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="dc786-114">permitiu</span><span class="sxs-lookup"><span data-stu-id="dc786-114">allow</span></span>|<span data-ttu-id="dc786-115">1</span><span class="sxs-lookup"><span data-stu-id="dc786-115">1</span></span>|<span data-ttu-id="dc786-116">O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="dc786-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="dc786-117">O Intune não tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="dc786-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="dc786-118">eliminação</span><span class="sxs-lookup"><span data-stu-id="dc786-118">suppress</span></span>|<span data-ttu-id="dc786-119">duas</span><span class="sxs-lookup"><span data-stu-id="dc786-119">2</span></span>|<span data-ttu-id="dc786-120">O Intune tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="dc786-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="dc786-121">vigor</span><span class="sxs-lookup"><span data-stu-id="dc786-121">force</span></span>|<span data-ttu-id="dc786-122">3D</span><span class="sxs-lookup"><span data-stu-id="dc786-122">3</span></span>|<span data-ttu-id="dc786-123">O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc786-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|



