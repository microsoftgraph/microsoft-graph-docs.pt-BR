---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00909f739773e67d4b5a1ae87f53982b627f511e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809166"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="5edb9-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="5edb9-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="5edb9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5edb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5edb9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5edb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5edb9-106">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="5edb9-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="5edb9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5edb9-107">Members</span></span>
|<span data-ttu-id="5edb9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5edb9-108">Member</span></span>|<span data-ttu-id="5edb9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5edb9-109">Value</span></span>|<span data-ttu-id="5edb9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5edb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5edb9-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5edb9-111">notConfigured</span></span>|<span data-ttu-id="5edb9-112">,0</span><span class="sxs-lookup"><span data-stu-id="5edb9-112">0</span></span>|<span data-ttu-id="5edb9-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="5edb9-113">Not Configured</span></span>|
|<span data-ttu-id="5edb9-114">permissão</span><span class="sxs-lookup"><span data-stu-id="5edb9-114">allowList</span></span>|<span data-ttu-id="5edb9-115">1</span><span class="sxs-lookup"><span data-stu-id="5edb9-115">1</span></span>|<span data-ttu-id="5edb9-116">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5edb9-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="5edb9-117">Lista</span><span class="sxs-lookup"><span data-stu-id="5edb9-117">blockList</span></span>|<span data-ttu-id="5edb9-118">duas</span><span class="sxs-lookup"><span data-stu-id="5edb9-118">2</span></span>|<span data-ttu-id="5edb9-119">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="5edb9-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|





