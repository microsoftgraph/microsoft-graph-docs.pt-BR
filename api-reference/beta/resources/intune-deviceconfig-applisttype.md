---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b7d11107ca3ea2b698e28cd288f163ec190b0a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172671"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="297e0-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="297e0-103">appListType enum type</span></span>

> <span data-ttu-id="297e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="297e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="297e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="297e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="297e0-106">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="297e0-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="297e0-107">Membros</span><span class="sxs-lookup"><span data-stu-id="297e0-107">Members</span></span>
|<span data-ttu-id="297e0-108">Membro</span><span class="sxs-lookup"><span data-stu-id="297e0-108">Member</span></span>|<span data-ttu-id="297e0-109">Valor</span><span class="sxs-lookup"><span data-stu-id="297e0-109">Value</span></span>|<span data-ttu-id="297e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="297e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297e0-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="297e0-111">none</span></span>|<span data-ttu-id="297e0-112">,0</span><span class="sxs-lookup"><span data-stu-id="297e0-112">0</span></span>|<span data-ttu-id="297e0-113">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="297e0-113">Default value, no intent.</span></span>|
|<span data-ttu-id="297e0-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="297e0-114">appsInListCompliant</span></span>|<span data-ttu-id="297e0-115">1</span><span class="sxs-lookup"><span data-stu-id="297e0-115">1</span></span>|<span data-ttu-id="297e0-116">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="297e0-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="297e0-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="297e0-117">appsNotInListCompliant</span></span>|<span data-ttu-id="297e0-118">duas</span><span class="sxs-lookup"><span data-stu-id="297e0-118">2</span></span>|<span data-ttu-id="297e0-119">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="297e0-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




