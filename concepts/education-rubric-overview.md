---
title: Visão geral do Rubric Education
description: O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: 56b9bcdf32036361fb92fe372952c94d09d8dc57
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173080"
---
# <a name="education-rubric-overview"></a>Visão geral do Rubric Education

O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.

Uma rubric de gradação é uma matriz de *qualidades*,*níveis*, e *critérios*, da seguinte maneira:

| | Nível | Nível |
|:--|:--|:--|
| Qualidade | Critério | Critério |
| Qualidade | Critério | Critério |

Um exemplo de um rubric de gradação pode ser:

| | Good | Ruim |
|:--|:--|:--|
| Argumento | O argumento de ensaio é persuasivo. | O argumento de ensaio não faz sentido. |
| Ortografia e Gramática | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

A gradação usando uma rubric envolve a seleção de um *nível* para cada *qualidade* no rubric.

Um rubric *pode* ter pontos associados a todos os níveis e uma gramatura associada a cada qualidade.  Se houver, os pesos devem adicionar até 100.

| | Bom (2 pontos) | Baixo (1 ponto) |
|:--|:--|:--|
| Argumento (peso 50) | O argumento de ensaio é persuasivo. | O argumento de ensaio não faz sentido. |
| Ortografia e gramática (peso 50) | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

## <a name="api-reference"></a>Referência da API

Para começar a usar o rubrics, comece [com o recurso educationRubric no Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) e os métodos associados.





 

