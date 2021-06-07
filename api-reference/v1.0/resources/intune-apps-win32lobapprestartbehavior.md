---
title: Tipo denum win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc6ff030c2228ae108e034eea312c57d40b9006f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758964"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="0445f-103">Tipo denum win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="0445f-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="0445f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0445f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0445f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0445f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0445f-106">Indica o tipo de ação de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="0445f-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="0445f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0445f-107">Members</span></span>
|<span data-ttu-id="0445f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0445f-108">Member</span></span>|<span data-ttu-id="0445f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0445f-109">Value</span></span>|<span data-ttu-id="0445f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0445f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0445f-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="0445f-111">basedOnReturnCode</span></span>|<span data-ttu-id="0445f-112">0</span><span class="sxs-lookup"><span data-stu-id="0445f-112">0</span></span>|<span data-ttu-id="0445f-113">O Intune reiniciará o dispositivo após executar a instalação do aplicativo se a operação retornar um código de reinicialização.</span><span class="sxs-lookup"><span data-stu-id="0445f-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="0445f-114">allow</span><span class="sxs-lookup"><span data-stu-id="0445f-114">allow</span></span>|<span data-ttu-id="0445f-115">1</span><span class="sxs-lookup"><span data-stu-id="0445f-115">1</span></span>|<span data-ttu-id="0445f-116">O Intune não tomará nenhuma ação específica sobre códigos de reinicialização resultantes de instalações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0445f-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="0445f-117">O Intune não tentará suprimir reinicializações para aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="0445f-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="0445f-118">suppress</span><span class="sxs-lookup"><span data-stu-id="0445f-118">suppress</span></span>|<span data-ttu-id="0445f-119">2</span><span class="sxs-lookup"><span data-stu-id="0445f-119">2</span></span>|<span data-ttu-id="0445f-120">O Intune tentará suprimir reinicializações para aplicativos MSI.</span><span class="sxs-lookup"><span data-stu-id="0445f-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="0445f-121">force</span><span class="sxs-lookup"><span data-stu-id="0445f-121">force</span></span>|<span data-ttu-id="0445f-122">3</span><span class="sxs-lookup"><span data-stu-id="0445f-122">3</span></span>|<span data-ttu-id="0445f-123">O Intune força o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0445f-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|




