---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9cee18df0fe6ba3cc59d8d427aa472f8943e03d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527789"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="bbb86-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="bbb86-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="bbb86-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbb86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbb86-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbb86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbb86-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbb86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb86-107">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="bbb86-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="bbb86-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bbb86-108">Members</span></span>
|<span data-ttu-id="bbb86-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bbb86-109">Member</span></span>|<span data-ttu-id="bbb86-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bbb86-110">Value</span></span>|<span data-ttu-id="bbb86-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb86-112">active</span><span class="sxs-lookup"><span data-stu-id="bbb86-112">active</span></span>|<span data-ttu-id="bbb86-113">,0</span><span class="sxs-lookup"><span data-stu-id="bbb86-113">0</span></span>|<span data-ttu-id="bbb86-114">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="bbb86-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="bbb86-115">erro</span><span class="sxs-lookup"><span data-stu-id="bbb86-115">error</span></span>|<span data-ttu-id="bbb86-116">1 </span><span class="sxs-lookup"><span data-stu-id="bbb86-116">1</span></span>|<span data-ttu-id="bbb86-117">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="bbb86-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="bbb86-118">inativa</span><span class="sxs-lookup"><span data-stu-id="bbb86-118">inactive</span></span>|<span data-ttu-id="bbb86-119">2 </span><span class="sxs-lookup"><span data-stu-id="bbb86-119">2</span></span>|<span data-ttu-id="bbb86-120">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="bbb86-120">There is no heart-beat from connector from last 5 days.</span></span>|



