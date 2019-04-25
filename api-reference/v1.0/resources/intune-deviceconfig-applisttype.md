---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575097"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="2ec4f-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="2ec4f-103">appListType enum type</span></span>

> <span data-ttu-id="2ec4f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ec4f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ec4f-105">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2ec4f-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="2ec4f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2ec4f-106">Members</span></span>
|<span data-ttu-id="2ec4f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2ec4f-107">Member</span></span>|<span data-ttu-id="2ec4f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2ec4f-108">Value</span></span>|<span data-ttu-id="2ec4f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec4f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ec4f-110">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2ec4f-110">none</span></span>|<span data-ttu-id="2ec4f-111">,0</span><span class="sxs-lookup"><span data-stu-id="2ec4f-111">0</span></span>|<span data-ttu-id="2ec4f-112">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="2ec4f-112">Default value, no intent.</span></span>|
|<span data-ttu-id="2ec4f-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2ec4f-113">appsInListCompliant</span></span>|<span data-ttu-id="2ec4f-114">1 </span><span class="sxs-lookup"><span data-stu-id="2ec4f-114">1</span></span>|<span data-ttu-id="2ec4f-115">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="2ec4f-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="2ec4f-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2ec4f-116">appsNotInListCompliant</span></span>|<span data-ttu-id="2ec4f-117">2 </span><span class="sxs-lookup"><span data-stu-id="2ec4f-117">2</span></span>|<span data-ttu-id="2ec4f-118">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="2ec4f-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



