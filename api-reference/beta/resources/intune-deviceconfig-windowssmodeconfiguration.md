---
title: tipo de enumeração windowsSModeConfiguration
description: As opções possíveis para configurar o desbloqueio de modo S
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7358f7067a868dd891b701f2d67c9abc5fbd422c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684852"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="6a351-103">tipo de enumeração windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a351-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="6a351-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a351-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a351-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a351-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a351-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a351-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a351-107">As opções possíveis para configurar o desbloqueio de modo S</span><span class="sxs-lookup"><span data-stu-id="6a351-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="6a351-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6a351-108">Members</span></span>
|<span data-ttu-id="6a351-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6a351-109">Member</span></span>|<span data-ttu-id="6a351-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6a351-110">Value</span></span>|<span data-ttu-id="6a351-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a351-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a351-112">restrict</span><span class="sxs-lookup"><span data-stu-id="6a351-112">noRestriction</span></span>|<span data-ttu-id="6a351-113">,0</span><span class="sxs-lookup"><span data-stu-id="6a351-113">0</span></span>|<span data-ttu-id="6a351-114">Essa opção removerá todas as restrições para desbloquear o modo S-padrão</span><span class="sxs-lookup"><span data-stu-id="6a351-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="6a351-115">Larga</span><span class="sxs-lookup"><span data-stu-id="6a351-115">block</span></span>|<span data-ttu-id="6a351-116">1</span><span class="sxs-lookup"><span data-stu-id="6a351-116">1</span></span>|<span data-ttu-id="6a351-117">Essa opção impedirá que o usuário desbloqueie o dispositivo no modo S</span><span class="sxs-lookup"><span data-stu-id="6a351-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="6a351-118">bloqueio</span><span class="sxs-lookup"><span data-stu-id="6a351-118">unlock</span></span>|<span data-ttu-id="6a351-119">duas</span><span class="sxs-lookup"><span data-stu-id="6a351-119">2</span></span>|<span data-ttu-id="6a351-120">Essa opção destravará o dispositivo do modo S</span><span class="sxs-lookup"><span data-stu-id="6a351-120">This option will unlock the device from S mode</span></span>|





