---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58b0a3a9e590913d0415062d6737fc6d9c33c451
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222755"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="af363-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="af363-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="af363-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af363-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af363-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af363-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af363-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af363-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af363-107">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="af363-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="af363-108">Membros</span><span class="sxs-lookup"><span data-stu-id="af363-108">Members</span></span>
|<span data-ttu-id="af363-109">Membro</span><span class="sxs-lookup"><span data-stu-id="af363-109">Member</span></span>|<span data-ttu-id="af363-110">Valor</span><span class="sxs-lookup"><span data-stu-id="af363-110">Value</span></span>|<span data-ttu-id="af363-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="af363-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af363-112">active</span><span class="sxs-lookup"><span data-stu-id="af363-112">active</span></span>|<span data-ttu-id="af363-113">,0</span><span class="sxs-lookup"><span data-stu-id="af363-113">0</span></span>|<span data-ttu-id="af363-114">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="af363-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="af363-115">erro</span><span class="sxs-lookup"><span data-stu-id="af363-115">error</span></span>|<span data-ttu-id="af363-116">1</span><span class="sxs-lookup"><span data-stu-id="af363-116">1</span></span>|<span data-ttu-id="af363-117">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="af363-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="af363-118">inativa</span><span class="sxs-lookup"><span data-stu-id="af363-118">inactive</span></span>|<span data-ttu-id="af363-119">duas</span><span class="sxs-lookup"><span data-stu-id="af363-119">2</span></span>|<span data-ttu-id="af363-120">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="af363-120">There is no heart-beat from connector from last 5 days.</span></span>|




