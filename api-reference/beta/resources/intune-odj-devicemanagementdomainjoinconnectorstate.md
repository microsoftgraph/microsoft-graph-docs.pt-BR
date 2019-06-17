---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001913"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="5533a-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="5533a-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="5533a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5533a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5533a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5533a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5533a-106">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="5533a-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="5533a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5533a-107">Members</span></span>
|<span data-ttu-id="5533a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5533a-108">Member</span></span>|<span data-ttu-id="5533a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5533a-109">Value</span></span>|<span data-ttu-id="5533a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5533a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5533a-111">active</span><span class="sxs-lookup"><span data-stu-id="5533a-111">active</span></span>|<span data-ttu-id="5533a-112">,0</span><span class="sxs-lookup"><span data-stu-id="5533a-112">0</span></span>|<span data-ttu-id="5533a-113">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="5533a-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="5533a-114">erro</span><span class="sxs-lookup"><span data-stu-id="5533a-114">error</span></span>|<span data-ttu-id="5533a-115">1</span><span class="sxs-lookup"><span data-stu-id="5533a-115">1</span></span>|<span data-ttu-id="5533a-116">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="5533a-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="5533a-117">inativa</span><span class="sxs-lookup"><span data-stu-id="5533a-117">inactive</span></span>|<span data-ttu-id="5533a-118">duas</span><span class="sxs-lookup"><span data-stu-id="5533a-118">2</span></span>|<span data-ttu-id="5533a-119">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="5533a-119">There is no heart-beat from connector from last 5 days.</span></span>|





