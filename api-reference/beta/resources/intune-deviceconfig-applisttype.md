---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a05fc37f692d58a4d5d434037fd9d1ebe09ecaa9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798723"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="df053-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="df053-103">appListType enum type</span></span>

> <span data-ttu-id="df053-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df053-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df053-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df053-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df053-106">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="df053-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="df053-107">Membros</span><span class="sxs-lookup"><span data-stu-id="df053-107">Members</span></span>
|<span data-ttu-id="df053-108">Membro</span><span class="sxs-lookup"><span data-stu-id="df053-108">Member</span></span>|<span data-ttu-id="df053-109">Valor</span><span class="sxs-lookup"><span data-stu-id="df053-109">Value</span></span>|<span data-ttu-id="df053-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df053-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df053-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="df053-111">none</span></span>|<span data-ttu-id="df053-112">,0</span><span class="sxs-lookup"><span data-stu-id="df053-112">0</span></span>|<span data-ttu-id="df053-113">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="df053-113">Default value, no intent.</span></span>|
|<span data-ttu-id="df053-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="df053-114">appsInListCompliant</span></span>|<span data-ttu-id="df053-115">1</span><span class="sxs-lookup"><span data-stu-id="df053-115">1</span></span>|<span data-ttu-id="df053-116">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="df053-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="df053-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="df053-117">appsNotInListCompliant</span></span>|<span data-ttu-id="df053-118">duas</span><span class="sxs-lookup"><span data-stu-id="df053-118">2</span></span>|<span data-ttu-id="df053-119">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="df053-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





