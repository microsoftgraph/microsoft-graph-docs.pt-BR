---
title: Visão geral do Rubric Education
description: O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.
author: mmast-msft
ms.localizationpriority: high
ms.prod: education
ms.openlocfilehash: 6df1ad373de6e0f6f5fe59b0a4b3e48a68bcf0e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137389"
---
# <a name="education-rubric-overview"></a>Visão geral do Rubric Education

O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.

Uma rubric de gradação é uma matriz de *qualidades*,*níveis*, e *critérios*, da seguinte maneira:

| &nbsp;  | Nível     | Nível     |
|:--------|:----------|:----------|
| Qualidade | Critério | Critério |
| Qualidade | Critério | Critério |

Um exemplo de um rubric de gradação pode ser:

| &nbsp;               | Good                                                              | Ruim                                                      |
|:---------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| Argumento             | O argumento de ensaio é persuasivo.                               | O argumento de ensaio não faz sentido.                 |
| Ortografia e Gramática | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

A gradação usando uma rubric envolve a seleção de um *nível* para cada *qualidade* no rubric.

Um rubric *pode* ter pontos associados a todos os níveis e uma gramatura associada a cada qualidade.  Se houver, os pesos devem adicionar até 100.

| &nbsp;                           | Bom (2 pontos)                                                   | Baixo (1 ponto)                                            |
|:---------------------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| Argumento (peso 50)             | O argumento de ensaio é persuasivo.                               | O argumento de ensaio não faz sentido.                 |
| Ortografia e gramática (peso 50) | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

## <a name="api-reference"></a>Referência da API

Para começar a usar o rubrics, comece [com o recurso educationRubric no Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) e os métodos associados.
