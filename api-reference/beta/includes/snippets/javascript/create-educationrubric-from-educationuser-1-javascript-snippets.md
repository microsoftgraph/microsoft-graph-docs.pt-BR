---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 267204bbdb5db20fd8c16825f84b4d4c388c95bd36199096c4f817567291ae38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
    displayName: 'Example Credit Rubric',
    description: {
        content: 'This is an example of a credit rubric (no points)',
        contentType: 'text'
    },
    levels: [
        {
            displayName: 'Good',
            description: {
                content: '',
                contentType: 'text'
            }
        },
        {
            displayName: 'Poor',
            description: {
                content: '',
                contentType: 'text'
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
            ]
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
            ]
        }
    ]
};

await client.api('/education/me/rubrics')
    .version('beta')
    .post(educationRubric);

```