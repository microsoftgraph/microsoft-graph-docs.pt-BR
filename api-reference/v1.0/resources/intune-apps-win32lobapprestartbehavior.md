---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a4f9044e90c67afe3ec50ba2349a94d194641dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036695"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="4f407-103">tipo de enumeração win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="4f407-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="4f407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f407-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f407-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f407-106">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="4f407-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="4f407-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4f407-107">Members</span></span>
|<span data-ttu-id="4f407-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4f407-108">Member</span></span>|<span data-ttu-id="4f407-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4f407-109">Value</span></span>|<span data-ttu-id="4f407-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f407-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f407-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="4f407-111">basedOnReturnCode</span></span>|<span data-ttu-id="4f407-112">,0</span><span class="sxs-lookup"><span data-stu-id="4f407-112">0</span></span>|<span data-ttu-id="4f407-113">O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="4f407-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="4f407-114">permitiu</span><span class="sxs-lookup"><span data-stu-id="4f407-114">allow</span></span>|<span data-ttu-id="4f407-115">1 </span><span class="sxs-lookup"><span data-stu-id="4f407-115">1</span></span>|<span data-ttu-id="4f407-116">O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4f407-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="4f407-117">O Intune não tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="4f407-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="4f407-118">eliminação</span><span class="sxs-lookup"><span data-stu-id="4f407-118">suppress</span></span>|<span data-ttu-id="4f407-119">2 </span><span class="sxs-lookup"><span data-stu-id="4f407-119">2</span></span>|<span data-ttu-id="4f407-120">O Intune tentará suprimir as reinicializações para os aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="4f407-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="4f407-121">vigor</span><span class="sxs-lookup"><span data-stu-id="4f407-121">force</span></span>|<span data-ttu-id="4f407-122">3 </span><span class="sxs-lookup"><span data-stu-id="4f407-122">3</span></span>|<span data-ttu-id="4f407-123">O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f407-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|





