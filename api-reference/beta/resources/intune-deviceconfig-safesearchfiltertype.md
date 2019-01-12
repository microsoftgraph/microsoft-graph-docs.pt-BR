---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49252525b3c6bcab6fd79a1ed7c27b3004665fe8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944793"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="71ace-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="71ace-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="71ace-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71ace-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71ace-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71ace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71ace-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71ace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71ace-107">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="71ace-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="71ace-108">Membros</span><span class="sxs-lookup"><span data-stu-id="71ace-108">Members</span></span>
|<span data-ttu-id="71ace-109">Membro</span><span class="sxs-lookup"><span data-stu-id="71ace-109">Member</span></span>|<span data-ttu-id="71ace-110">Valor</span><span class="sxs-lookup"><span data-stu-id="71ace-110">Value</span></span>|<span data-ttu-id="71ace-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ace-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="71ace-112">userDefined</span></span>|<span data-ttu-id="71ace-113">0</span><span class="sxs-lookup"><span data-stu-id="71ace-113">0</span></span>|<span data-ttu-id="71ace-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="71ace-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="71ace-115">estrito</span><span class="sxs-lookup"><span data-stu-id="71ace-115">strict</span></span>|<span data-ttu-id="71ace-116">1</span><span class="sxs-lookup"><span data-stu-id="71ace-116">1</span></span>|<span data-ttu-id="71ace-117">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="71ace-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="71ace-118">moderar</span><span class="sxs-lookup"><span data-stu-id="71ace-118">moderate</span></span>|<span data-ttu-id="71ace-119">2</span><span class="sxs-lookup"><span data-stu-id="71ace-119">2</span></span>|<span data-ttu-id="71ace-120">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="71ace-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





