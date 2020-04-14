---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7f9f0aece71da72c2f10e23ac660a698a1f1439c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402816"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="40209-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="40209-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="40209-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40209-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40209-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40209-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40209-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40209-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40209-107">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="40209-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="40209-108">Membros</span><span class="sxs-lookup"><span data-stu-id="40209-108">Members</span></span>
|<span data-ttu-id="40209-109">Membro</span><span class="sxs-lookup"><span data-stu-id="40209-109">Member</span></span>|<span data-ttu-id="40209-110">Valor</span><span class="sxs-lookup"><span data-stu-id="40209-110">Value</span></span>|<span data-ttu-id="40209-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40209-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40209-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="40209-112">notConfigured</span></span>|<span data-ttu-id="40209-113">,0</span><span class="sxs-lookup"><span data-stu-id="40209-113">0</span></span>|<span data-ttu-id="40209-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="40209-114">Not Configured</span></span>|
|<span data-ttu-id="40209-115">permissão</span><span class="sxs-lookup"><span data-stu-id="40209-115">allowList</span></span>|<span data-ttu-id="40209-116">1</span><span class="sxs-lookup"><span data-stu-id="40209-116">1</span></span>|<span data-ttu-id="40209-117">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40209-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="40209-118">Lista</span><span class="sxs-lookup"><span data-stu-id="40209-118">blockList</span></span>|<span data-ttu-id="40209-119">duas</span><span class="sxs-lookup"><span data-stu-id="40209-119">2</span></span>|<span data-ttu-id="40209-120">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="40209-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



