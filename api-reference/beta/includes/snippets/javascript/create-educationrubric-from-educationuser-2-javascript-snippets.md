---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9264f85e738c9af526de34028c07217bbc1e7d9fdd9cc9873145c2fec19fc8ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
    displayName: 'Example Points Rubric',
    description: {
        content: 'This is an example of a rubric with points',
        contentType: 'text'
    },
    levels: [
        {
            displayName: 'Good',
            description: {
                content: '',
                contentType: 'text'
            },
            grading: {
                '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType',
                maxPoints: 2
            }
        },
        {
            displayName: 'Poor',
            description: {
                content: '',
                contentType: 'text'
            },
            grading: {
                '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType',
                maxPoints: 1
            }
        }
    ],
    qualities: [
        {
            description: {
                content: 'Argument',
                contentType: 'text'
            },
            criteria: [
                {
                    description: {
                        content: 'The essay\'s argument is persuasive.',
                        contentType: 'text'
                    }
                },
                {
                    description: {
                        content: 'The essay\'s argument does not make sense.',
                        contentType: 'text'
                    }
                }
            ],
            weight: 50.0
        },
        {
            description: {
                content: 'Spelling and Grammar',
                contentType: 'text'
            },
            criteria: [
                {
                    description: {
                        content: 'The essay uses proper spelling and grammar with few or no errors.',
                        contentType: 'text'
                    }
                },
                {
                    description: {
                        content: 'The essay has numerous errors in spelling and/or grammar.',
                        contentType: 'text'
                    }
                }
            ],
            weight: 50.0
        }
    ],
    grading: {
        '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType'
    }
};

await client.api('/education/me/rubrics')
    .version('beta')
    .post(educationRubric);

```