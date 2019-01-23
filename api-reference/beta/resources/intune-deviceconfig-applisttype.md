---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415219"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="14eca-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="14eca-103">appListType enum type</span></span>

> <span data-ttu-id="14eca-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="14eca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14eca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14eca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14eca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="14eca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14eca-107">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="14eca-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="14eca-108">Membros</span><span class="sxs-lookup"><span data-stu-id="14eca-108">Members</span></span>
|<span data-ttu-id="14eca-109">Membro</span><span class="sxs-lookup"><span data-stu-id="14eca-109">Member</span></span>|<span data-ttu-id="14eca-110">Valor</span><span class="sxs-lookup"><span data-stu-id="14eca-110">Value</span></span>|<span data-ttu-id="14eca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14eca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14eca-112">none</span><span class="sxs-lookup"><span data-stu-id="14eca-112">none</span></span>|<span data-ttu-id="14eca-113">0</span><span class="sxs-lookup"><span data-stu-id="14eca-113">0</span></span>|<span data-ttu-id="14eca-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="14eca-114">Default value, no intent.</span></span>|
|<span data-ttu-id="14eca-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="14eca-115">appsInListCompliant</span></span>|<span data-ttu-id="14eca-116">1</span><span class="sxs-lookup"><span data-stu-id="14eca-116">1</span></span>|<span data-ttu-id="14eca-117">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="14eca-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="14eca-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="14eca-118">appsNotInListCompliant</span></span>|<span data-ttu-id="14eca-119">2</span><span class="sxs-lookup"><span data-stu-id="14eca-119">2</span></span>|<span data-ttu-id="14eca-120">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="14eca-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




