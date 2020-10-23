---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 97f1579e0a3bec8b063bba5e1a95cc92ba637c9a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691159"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="b48da-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="b48da-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="b48da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b48da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b48da-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b48da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b48da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b48da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b48da-107">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="b48da-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="b48da-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b48da-108">Members</span></span>
|<span data-ttu-id="b48da-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b48da-109">Member</span></span>|<span data-ttu-id="b48da-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b48da-110">Value</span></span>|<span data-ttu-id="b48da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b48da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b48da-112">active</span><span class="sxs-lookup"><span data-stu-id="b48da-112">active</span></span>|<span data-ttu-id="b48da-113">,0</span><span class="sxs-lookup"><span data-stu-id="b48da-113">0</span></span>|<span data-ttu-id="b48da-114">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="b48da-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="b48da-115">erro</span><span class="sxs-lookup"><span data-stu-id="b48da-115">error</span></span>|<span data-ttu-id="b48da-116">1</span><span class="sxs-lookup"><span data-stu-id="b48da-116">1</span></span>|<span data-ttu-id="b48da-117">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="b48da-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="b48da-118">inativa</span><span class="sxs-lookup"><span data-stu-id="b48da-118">inactive</span></span>|<span data-ttu-id="b48da-119">duas</span><span class="sxs-lookup"><span data-stu-id="b48da-119">2</span></span>|<span data-ttu-id="b48da-120">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="b48da-120">There is no heart-beat from connector from last 5 days.</span></span>|





