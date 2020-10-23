---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 79bf27c55b1bb237cac8c537473e8ffd98edca7a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708820"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="48a91-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="48a91-103">appListType enum type</span></span>

<span data-ttu-id="48a91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48a91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48a91-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48a91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48a91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48a91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48a91-107">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="48a91-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="48a91-108">Membros</span><span class="sxs-lookup"><span data-stu-id="48a91-108">Members</span></span>
|<span data-ttu-id="48a91-109">Membro</span><span class="sxs-lookup"><span data-stu-id="48a91-109">Member</span></span>|<span data-ttu-id="48a91-110">Valor</span><span class="sxs-lookup"><span data-stu-id="48a91-110">Value</span></span>|<span data-ttu-id="48a91-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48a91-112">none</span><span class="sxs-lookup"><span data-stu-id="48a91-112">none</span></span>|<span data-ttu-id="48a91-113">,0</span><span class="sxs-lookup"><span data-stu-id="48a91-113">0</span></span>|<span data-ttu-id="48a91-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="48a91-114">Default value, no intent.</span></span>|
|<span data-ttu-id="48a91-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="48a91-115">appsInListCompliant</span></span>|<span data-ttu-id="48a91-116">1</span><span class="sxs-lookup"><span data-stu-id="48a91-116">1</span></span>|<span data-ttu-id="48a91-117">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="48a91-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="48a91-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="48a91-118">appsNotInListCompliant</span></span>|<span data-ttu-id="48a91-119">duas</span><span class="sxs-lookup"><span data-stu-id="48a91-119">2</span></span>|<span data-ttu-id="48a91-120">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="48a91-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





