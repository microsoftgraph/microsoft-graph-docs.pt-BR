---
title: Visão geral do Rubric Education
description: O Rubrics é uma maneira eficaz e amplamente utilizada de gradação de tarefas, e a API Education no Microsoft Graph dá suporte a elas.
author: mmast-msft
ms.localizationpriority: high
ms.prod: education
ms.openlocfilehash: 7ea10f339d6ee53b991045382bfcb5cbe1d27534
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440877"
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
| Ortografia e gramática | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

A gradação usando uma rubric envolve a seleção de um *nível* para cada *qualidade* no rubric.

Um rubric *pode* ter pontos associados a todos os níveis e uma gramatura associada a cada qualidade.  Se houver, os pesos devem adicionar até 100.

| &nbsp;                           | Bom (2 pontos)                                                   | Baixo (1 ponto)                                            |
|:---------------------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| Argumento (peso 50)             | O argumento de ensaio é persuasivo.                               | O argumento de ensaio não faz sentido.                 |
| Ortografia e gramática (peso 50) | O ensaio usa a verificação ortográfica e gramatical adequada com poucos erros. | O ensaio tem vários erros de ortografia e/ou gramática. |

## <a name="api-reference"></a>Referência da API

Para começar a usar o rubrics, comece com o recurso [educationRubric no Microsoft Graph](/graph/api/resources/educationrubric) beta e os métodos associados.
