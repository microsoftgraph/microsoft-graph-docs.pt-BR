---
title: tipo de enumeração windowsSModeConfiguration
description: As opções possíveis para configurar o desbloqueio de modo S
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd9b4c696c7456e4cf926764bfadde3fbd591a6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525401"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="41683-103">tipo de enumeração windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="41683-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="41683-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41683-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41683-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41683-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41683-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41683-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41683-107">As opções possíveis para configurar o desbloqueio de modo S</span><span class="sxs-lookup"><span data-stu-id="41683-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="41683-108">Membros</span><span class="sxs-lookup"><span data-stu-id="41683-108">Members</span></span>
|<span data-ttu-id="41683-109">Membro</span><span class="sxs-lookup"><span data-stu-id="41683-109">Member</span></span>|<span data-ttu-id="41683-110">Valor</span><span class="sxs-lookup"><span data-stu-id="41683-110">Value</span></span>|<span data-ttu-id="41683-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41683-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41683-112">restrict</span><span class="sxs-lookup"><span data-stu-id="41683-112">noRestriction</span></span>|<span data-ttu-id="41683-113">,0</span><span class="sxs-lookup"><span data-stu-id="41683-113">0</span></span>|<span data-ttu-id="41683-114">Essa opção removerá todas as restrições para desbloquear o modo S-padrão</span><span class="sxs-lookup"><span data-stu-id="41683-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="41683-115">Larga</span><span class="sxs-lookup"><span data-stu-id="41683-115">block</span></span>|<span data-ttu-id="41683-116">1 </span><span class="sxs-lookup"><span data-stu-id="41683-116">1</span></span>|<span data-ttu-id="41683-117">Essa opção impedirá que o usuário desbloqueie o dispositivo no modo S</span><span class="sxs-lookup"><span data-stu-id="41683-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="41683-118">bloqueio</span><span class="sxs-lookup"><span data-stu-id="41683-118">unlock</span></span>|<span data-ttu-id="41683-119">2 </span><span class="sxs-lookup"><span data-stu-id="41683-119">2</span></span>|<span data-ttu-id="41683-120">Essa opção destravará o dispositivo do modo S</span><span class="sxs-lookup"><span data-stu-id="41683-120">This option will unlock the device from S mode</span></span>|



