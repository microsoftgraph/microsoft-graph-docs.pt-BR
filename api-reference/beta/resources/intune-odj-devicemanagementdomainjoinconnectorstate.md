---
title: tipo de enumeração deviceManagementDomainJoinConnectorState
description: A solicitação ODJ diz.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8eff02a8ff4d47f920bad6506bcb9e3b37f0785
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779881"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="f9bca-103">tipo de enumeração deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="f9bca-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="f9bca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9bca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9bca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9bca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9bca-106">A solicitação ODJ diz.</span><span class="sxs-lookup"><span data-stu-id="f9bca-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="f9bca-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f9bca-107">Members</span></span>
|<span data-ttu-id="f9bca-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f9bca-108">Member</span></span>|<span data-ttu-id="f9bca-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f9bca-109">Value</span></span>|<span data-ttu-id="f9bca-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9bca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9bca-111">active</span><span class="sxs-lookup"><span data-stu-id="f9bca-111">active</span></span>|<span data-ttu-id="f9bca-112">,0</span><span class="sxs-lookup"><span data-stu-id="f9bca-112">0</span></span>|<span data-ttu-id="f9bca-113">O conector está ativamente fazendo ping no Intune.</span><span class="sxs-lookup"><span data-stu-id="f9bca-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="f9bca-114">erro</span><span class="sxs-lookup"><span data-stu-id="f9bca-114">error</span></span>|<span data-ttu-id="f9bca-115">1</span><span class="sxs-lookup"><span data-stu-id="f9bca-115">1</span></span>|<span data-ttu-id="f9bca-116">Não há um coração do conector da última hora.</span><span class="sxs-lookup"><span data-stu-id="f9bca-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="f9bca-117">inativa</span><span class="sxs-lookup"><span data-stu-id="f9bca-117">inactive</span></span>|<span data-ttu-id="f9bca-118">duas</span><span class="sxs-lookup"><span data-stu-id="f9bca-118">2</span></span>|<span data-ttu-id="f9bca-119">Não há um coração do conector dos últimos 5 dias.</span><span class="sxs-lookup"><span data-stu-id="f9bca-119">There is no heart-beat from connector from last 5 days.</span></span>|



