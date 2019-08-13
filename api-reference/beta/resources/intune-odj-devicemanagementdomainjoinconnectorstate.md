---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f664a6b57d92f5a8cd2d586f8bc2747ffa6db71c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342002"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="5e6b1-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="5e6b1-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="5e6b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e6b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e6b1-106">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="5e6b1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5e6b1-107">Members</span></span>
|<span data-ttu-id="5e6b1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5e6b1-108">Member</span></span>|<span data-ttu-id="5e6b1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5e6b1-109">Value</span></span>|<span data-ttu-id="5e6b1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e6b1-111">active</span><span class="sxs-lookup"><span data-stu-id="5e6b1-111">active</span></span>|<span data-ttu-id="5e6b1-112">,0</span><span class="sxs-lookup"><span data-stu-id="5e6b1-112">0</span></span>|<span data-ttu-id="5e6b1-113">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="5e6b1-114">erro</span><span class="sxs-lookup"><span data-stu-id="5e6b1-114">error</span></span>|<span data-ttu-id="5e6b1-115">1</span><span class="sxs-lookup"><span data-stu-id="5e6b1-115">1</span></span>|<span data-ttu-id="5e6b1-116">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="5e6b1-117">inativa</span><span class="sxs-lookup"><span data-stu-id="5e6b1-117">inactive</span></span>|<span data-ttu-id="5e6b1-118">duas</span><span class="sxs-lookup"><span data-stu-id="5e6b1-118">2</span></span>|<span data-ttu-id="5e6b1-119">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="5e6b1-119">There is no heart-beat from connector from last 5 days.</span></span>|



