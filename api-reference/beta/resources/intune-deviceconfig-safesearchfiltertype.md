---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4493c71b48a0f5ff4b0c48307504087c722393e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403480"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ab361-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="ab361-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ab361-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab361-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab361-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab361-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab361-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ab361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab361-107">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="ab361-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="ab361-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ab361-108">Members</span></span>
|<span data-ttu-id="ab361-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ab361-109">Member</span></span>|<span data-ttu-id="ab361-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ab361-110">Value</span></span>|<span data-ttu-id="ab361-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab361-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="ab361-112">userDefined</span></span>|<span data-ttu-id="ab361-113">0</span><span class="sxs-lookup"><span data-stu-id="ab361-113">0</span></span>|<span data-ttu-id="ab361-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="ab361-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ab361-115">estrito</span><span class="sxs-lookup"><span data-stu-id="ab361-115">strict</span></span>|<span data-ttu-id="ab361-116">1</span><span class="sxs-lookup"><span data-stu-id="ab361-116">1</span></span>|<span data-ttu-id="ab361-117">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="ab361-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ab361-118">moderar</span><span class="sxs-lookup"><span data-stu-id="ab361-118">moderate</span></span>|<span data-ttu-id="ab361-119">2</span><span class="sxs-lookup"><span data-stu-id="ab361-119">2</span></span>|<span data-ttu-id="ab361-120">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="ab361-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




