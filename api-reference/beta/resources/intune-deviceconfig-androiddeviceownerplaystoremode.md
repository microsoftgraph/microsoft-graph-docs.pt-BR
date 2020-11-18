---
title: tipo de enumeração androidDeviceOwnerPlayStoreMode
description: Tipo de modo de repositório de execução do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 899f3fab4bd0e6172b7fd16182d8195c427deb23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199956"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="473c3-103">tipo de enumeração androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="473c3-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="473c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="473c3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="473c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="473c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="473c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="473c3-107">Tipo de modo de repositório de execução do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="473c3-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="473c3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="473c3-108">Members</span></span>
|<span data-ttu-id="473c3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="473c3-109">Member</span></span>|<span data-ttu-id="473c3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="473c3-110">Value</span></span>|<span data-ttu-id="473c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="473c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="473c3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="473c3-112">notConfigured</span></span>|<span data-ttu-id="473c3-113">,0</span><span class="sxs-lookup"><span data-stu-id="473c3-113">0</span></span>|<span data-ttu-id="473c3-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="473c3-114">Not Configured</span></span>|
|<span data-ttu-id="473c3-115">permissão</span><span class="sxs-lookup"><span data-stu-id="473c3-115">allowList</span></span>|<span data-ttu-id="473c3-116">1</span><span class="sxs-lookup"><span data-stu-id="473c3-116">1</span></span>|<span data-ttu-id="473c3-117">Somente os aplicativos que estão na política estão disponíveis e qualquer aplicativo que não esteja na política será desinstalado automaticamente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="473c3-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="473c3-118">Lista</span><span class="sxs-lookup"><span data-stu-id="473c3-118">blockList</span></span>|<span data-ttu-id="473c3-119">duas</span><span class="sxs-lookup"><span data-stu-id="473c3-119">2</span></span>|<span data-ttu-id="473c3-120">Todos os aplicativos estão disponíveis e qualquer aplicativo que não esteja no dispositivo deve ser explicitamente marcado como ' bloqueado ' na política de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="473c3-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|




