---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 678a45d8ef75bc05d3093c086a65d66cb0cd174f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796997"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="e009a-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="e009a-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="e009a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e009a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e009a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e009a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e009a-106">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="e009a-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="e009a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e009a-107">Members</span></span>
|<span data-ttu-id="e009a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e009a-108">Member</span></span>|<span data-ttu-id="e009a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e009a-109">Value</span></span>|<span data-ttu-id="e009a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e009a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e009a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e009a-111">notConfigured</span></span>|<span data-ttu-id="e009a-112">,0</span><span class="sxs-lookup"><span data-stu-id="e009a-112">0</span></span>|<span data-ttu-id="e009a-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="e009a-113">Not Configured</span></span>|
|<span data-ttu-id="e009a-114">permissão</span><span class="sxs-lookup"><span data-stu-id="e009a-114">allowList</span></span>|<span data-ttu-id="e009a-115">1</span><span class="sxs-lookup"><span data-stu-id="e009a-115">1</span></span>|<span data-ttu-id="e009a-116">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e009a-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="e009a-117">Lista</span><span class="sxs-lookup"><span data-stu-id="e009a-117">blockList</span></span>|<span data-ttu-id="e009a-118">duas</span><span class="sxs-lookup"><span data-stu-id="e009a-118">2</span></span>|<span data-ttu-id="e009a-119">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e009a-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



