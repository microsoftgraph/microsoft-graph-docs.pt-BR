---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 96cc96d77de8b790208805dbf1a7f24a7858aa96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527087"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="246da-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="246da-103">appListType enum type</span></span>

<span data-ttu-id="246da-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="246da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="246da-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="246da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="246da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="246da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="246da-107">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="246da-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="246da-108">Membros</span><span class="sxs-lookup"><span data-stu-id="246da-108">Members</span></span>
|<span data-ttu-id="246da-109">Membro</span><span class="sxs-lookup"><span data-stu-id="246da-109">Member</span></span>|<span data-ttu-id="246da-110">Valor</span><span class="sxs-lookup"><span data-stu-id="246da-110">Value</span></span>|<span data-ttu-id="246da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="246da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="246da-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="246da-112">none</span></span>|<span data-ttu-id="246da-113">,0</span><span class="sxs-lookup"><span data-stu-id="246da-113">0</span></span>|<span data-ttu-id="246da-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="246da-114">Default value, no intent.</span></span>|
|<span data-ttu-id="246da-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="246da-115">appsInListCompliant</span></span>|<span data-ttu-id="246da-116">1 </span><span class="sxs-lookup"><span data-stu-id="246da-116">1</span></span>|<span data-ttu-id="246da-117">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="246da-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="246da-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="246da-118">appsNotInListCompliant</span></span>|<span data-ttu-id="246da-119">2 </span><span class="sxs-lookup"><span data-stu-id="246da-119">2</span></span>|<span data-ttu-id="246da-120">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="246da-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



