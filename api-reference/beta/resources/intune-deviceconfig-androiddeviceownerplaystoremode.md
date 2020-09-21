---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 802775fc56a3c961e03e757ac710abca35d8c8f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968700"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="c6995-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="c6995-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="c6995-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6995-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6995-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6995-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6995-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6995-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6995-107">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="c6995-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="c6995-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c6995-108">Members</span></span>
|<span data-ttu-id="c6995-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c6995-109">Member</span></span>|<span data-ttu-id="c6995-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c6995-110">Value</span></span>|<span data-ttu-id="c6995-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6995-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6995-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c6995-112">notConfigured</span></span>|<span data-ttu-id="c6995-113">,0</span><span class="sxs-lookup"><span data-stu-id="c6995-113">0</span></span>|<span data-ttu-id="c6995-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="c6995-114">Not Configured</span></span>|
|<span data-ttu-id="c6995-115">permissão</span><span class="sxs-lookup"><span data-stu-id="c6995-115">allowList</span></span>|<span data-ttu-id="c6995-116">1 </span><span class="sxs-lookup"><span data-stu-id="c6995-116">1</span></span>|<span data-ttu-id="c6995-117">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6995-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="c6995-118">Lista</span><span class="sxs-lookup"><span data-stu-id="c6995-118">blockList</span></span>|<span data-ttu-id="c6995-119">2 </span><span class="sxs-lookup"><span data-stu-id="c6995-119">2</span></span>|<span data-ttu-id="c6995-120">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="c6995-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|






