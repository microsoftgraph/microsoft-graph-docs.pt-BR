---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d883091a7162c7cb0da40113430edbdc66a9cfa7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334805"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="59e34-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="59e34-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="59e34-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59e34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59e34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59e34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59e34-106">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="59e34-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="59e34-107">Membros</span><span class="sxs-lookup"><span data-stu-id="59e34-107">Members</span></span>
|<span data-ttu-id="59e34-108">Membro</span><span class="sxs-lookup"><span data-stu-id="59e34-108">Member</span></span>|<span data-ttu-id="59e34-109">Valor</span><span class="sxs-lookup"><span data-stu-id="59e34-109">Value</span></span>|<span data-ttu-id="59e34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59e34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59e34-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="59e34-111">notConfigured</span></span>|<span data-ttu-id="59e34-112">,0</span><span class="sxs-lookup"><span data-stu-id="59e34-112">0</span></span>|<span data-ttu-id="59e34-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="59e34-113">Not Configured</span></span>|
|<span data-ttu-id="59e34-114">permissão</span><span class="sxs-lookup"><span data-stu-id="59e34-114">allowList</span></span>|<span data-ttu-id="59e34-115">1</span><span class="sxs-lookup"><span data-stu-id="59e34-115">1</span></span>|<span data-ttu-id="59e34-116">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59e34-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="59e34-117">Lista</span><span class="sxs-lookup"><span data-stu-id="59e34-117">blockList</span></span>|<span data-ttu-id="59e34-118">duas</span><span class="sxs-lookup"><span data-stu-id="59e34-118">2</span></span>|<span data-ttu-id="59e34-119">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="59e34-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



