---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a02b8ed105206f53894ddb8d35dc24106eebebc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028599"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="ef615-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="ef615-103">appListType enum type</span></span>

> <span data-ttu-id="ef615-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef615-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef615-105">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ef615-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="ef615-106">Membros</span><span class="sxs-lookup"><span data-stu-id="ef615-106">Members</span></span>
|<span data-ttu-id="ef615-107">Membro</span><span class="sxs-lookup"><span data-stu-id="ef615-107">Member</span></span>|<span data-ttu-id="ef615-108">Valor</span><span class="sxs-lookup"><span data-stu-id="ef615-108">Value</span></span>|<span data-ttu-id="ef615-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef615-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef615-110">none</span><span class="sxs-lookup"><span data-stu-id="ef615-110">none</span></span>|<span data-ttu-id="ef615-111">,0</span><span class="sxs-lookup"><span data-stu-id="ef615-111">0</span></span>|<span data-ttu-id="ef615-112">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="ef615-112">Default value, no intent.</span></span>|
|<span data-ttu-id="ef615-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ef615-113">appsInListCompliant</span></span>|<span data-ttu-id="ef615-114">1</span><span class="sxs-lookup"><span data-stu-id="ef615-114">1</span></span>|<span data-ttu-id="ef615-115">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="ef615-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="ef615-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ef615-116">appsNotInListCompliant</span></span>|<span data-ttu-id="ef615-117">duas</span><span class="sxs-lookup"><span data-stu-id="ef615-117">2</span></span>|<span data-ttu-id="ef615-118">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="ef615-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



