---
title: Visão geral do Rubric Education
description: O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: d17b325c12c75fbdd54d17a293aa6352707666e3
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845481"
---
# <a name="education-rubric-overview"></a><span data-ttu-id="3f38b-103">Visão geral do Rubric Education</span><span class="sxs-lookup"><span data-stu-id="3f38b-103">Education rubric overview</span></span>

<span data-ttu-id="3f38b-104">O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.</span><span class="sxs-lookup"><span data-stu-id="3f38b-104">Rubrics are an effective and widely-used way of grading assignments, and the education API in Microsoft Graph supports them.</span></span>

<span data-ttu-id="3f38b-105">Uma rubric de gradação é uma matriz de *qualidades*,*níveis*, e *critérios*, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="3f38b-105">A grading rubric is a matrix of *qualities*, *levels*, and *criteria*, as follows:</span></span>

| &nbsp;  | <span data-ttu-id="3f38b-106">Nível</span><span class="sxs-lookup"><span data-stu-id="3f38b-106">Level</span></span>     | <span data-ttu-id="3f38b-107">Nível</span><span class="sxs-lookup"><span data-stu-id="3f38b-107">Level</span></span>     |
|:--------|:----------|:----------|
| <span data-ttu-id="3f38b-108">Qualidade</span><span class="sxs-lookup"><span data-stu-id="3f38b-108">Quality</span></span> | <span data-ttu-id="3f38b-109">Critério</span><span class="sxs-lookup"><span data-stu-id="3f38b-109">Criterion</span></span> | <span data-ttu-id="3f38b-110">Critério</span><span class="sxs-lookup"><span data-stu-id="3f38b-110">Criterion</span></span> |
| <span data-ttu-id="3f38b-111">Qualidade</span><span class="sxs-lookup"><span data-stu-id="3f38b-111">Quality</span></span> | <span data-ttu-id="3f38b-112">Critério</span><span class="sxs-lookup"><span data-stu-id="3f38b-112">Criterion</span></span> | <span data-ttu-id="3f38b-113">Critério</span><span class="sxs-lookup"><span data-stu-id="3f38b-113">Criterion</span></span> |

<span data-ttu-id="3f38b-114">Um exemplo de um rubric de gradação pode ser:</span><span class="sxs-lookup"><span data-stu-id="3f38b-114">An example of a grading rubric might be:</span></span>

| &nbsp;               | <span data-ttu-id="3f38b-115">Good</span><span class="sxs-lookup"><span data-stu-id="3f38b-115">Good</span></span>                                                              | <span data-ttu-id="3f38b-116">Ruim</span><span class="sxs-lookup"><span data-stu-id="3f38b-116">Poor</span></span>                                                      |
|:---------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="3f38b-117">Argumento</span><span class="sxs-lookup"><span data-stu-id="3f38b-117">Argument</span></span>             | <span data-ttu-id="3f38b-118">O argumento de ensaio é persuasivo.</span><span class="sxs-lookup"><span data-stu-id="3f38b-118">The essay's argument is persuasive.</span></span>                               | <span data-ttu-id="3f38b-119">O argumento de ensaio não faz sentido.</span><span class="sxs-lookup"><span data-stu-id="3f38b-119">The essay's argument does not make sense.</span></span>                 |
| <span data-ttu-id="3f38b-120">Ortografia e Gramática</span><span class="sxs-lookup"><span data-stu-id="3f38b-120">Spelling and Grammar</span></span> | <span data-ttu-id="3f38b-121">O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros.</span><span class="sxs-lookup"><span data-stu-id="3f38b-121">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="3f38b-122">O ensaio tem vários erros de ortografia e/ou gramática.</span><span class="sxs-lookup"><span data-stu-id="3f38b-122">The essay has numerous errors in spelling and/or grammar.</span></span> |

<span data-ttu-id="3f38b-123">A gradação usando uma rubric envolve a seleção de um *nível* para cada *qualidade* no rubric.</span><span class="sxs-lookup"><span data-stu-id="3f38b-123">Grading using a rubric involves selecting one *level* for each *quality* in the rubric.</span></span>

<span data-ttu-id="3f38b-124">Um rubric *pode* ter pontos associados a todos os níveis e uma gramatura associada a cada qualidade.</span><span class="sxs-lookup"><span data-stu-id="3f38b-124">A rubric *may* have points associated with each level, and a weight associated with each quality.</span></span>  <span data-ttu-id="3f38b-125">Se houver, os pesos devem adicionar até 100.</span><span class="sxs-lookup"><span data-stu-id="3f38b-125">If present, weights must add up to 100.</span></span>

| &nbsp;                           | <span data-ttu-id="3f38b-126">Bom (2 pontos)</span><span class="sxs-lookup"><span data-stu-id="3f38b-126">Good (2 points)</span></span>                                                   | <span data-ttu-id="3f38b-127">Baixo (1 ponto)</span><span class="sxs-lookup"><span data-stu-id="3f38b-127">Poor (1 point)</span></span>                                            |
|:---------------------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="3f38b-128">Argumento (peso 50)</span><span class="sxs-lookup"><span data-stu-id="3f38b-128">Argument (weight 50)</span></span>             | <span data-ttu-id="3f38b-129">O argumento de ensaio é persuasivo.</span><span class="sxs-lookup"><span data-stu-id="3f38b-129">The essay's argument is persuasive.</span></span>                               | <span data-ttu-id="3f38b-130">O argumento de ensaio não faz sentido.</span><span class="sxs-lookup"><span data-stu-id="3f38b-130">The essay's argument does not make sense.</span></span>                 |
| <span data-ttu-id="3f38b-131">Ortografia e gramática (peso 50)</span><span class="sxs-lookup"><span data-stu-id="3f38b-131">Spelling and Grammar (weight 50)</span></span> | <span data-ttu-id="3f38b-132">O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros.</span><span class="sxs-lookup"><span data-stu-id="3f38b-132">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="3f38b-133">O ensaio tem vários erros de ortografia e/ou gramática.</span><span class="sxs-lookup"><span data-stu-id="3f38b-133">The essay has numerous errors in spelling and/or grammar.</span></span> |

## <a name="api-reference"></a><span data-ttu-id="3f38b-134">Referência da API</span><span class="sxs-lookup"><span data-stu-id="3f38b-134">API reference</span></span>

<span data-ttu-id="3f38b-135">Para começar a usar o rubrics, comece [com o recurso educationRubric no Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) e os métodos associados.</span><span class="sxs-lookup"><span data-stu-id="3f38b-135">To begin using rubrics, start with the [educationRubric resource in Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) and associated methods.</span></span>
