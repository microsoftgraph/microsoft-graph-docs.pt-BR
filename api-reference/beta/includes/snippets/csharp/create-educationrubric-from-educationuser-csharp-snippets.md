---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0543a2e2d6559fa0e268d412373affdbd8b62c80
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Points Rubric",
    Description = new EducationItemBody
    {
        Content = "This is an example of a rubric with points",
        ContentType = BodyType.Text
    },
    Levels = new List<RubricLevel>()
    {
        new RubricLevel
        {
            DisplayName = "Good",
            Description = new EducationItemBody
            {
                Content = "",
                ContentType = BodyType.Text
            },
            Grading = new EducationAssignmentPointsGradeType
            {
                MaxPoints = 2f
            }
        },
        new RubricLevel
        {
            DisplayName = "Poor",
            Description = new EducationItemBody
            {
                Content = "",
                ContentType = BodyType.Text
            },
            Grading = new EducationAssignmentPointsGradeType
            {
                MaxPoints = 1f
            }
        }
    },
    Qualities = new List<RubricQuality>()
    {
        new RubricQuality
        {
            Description = new EducationItemBody
            {
                Content = "Argument",
                ContentType = BodyType.Text
            },
            Criteria = new List<RubricCriterion>()
            {
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay's argument is persuasive.",
                        ContentType = BodyType.Text
                    }
                },
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay's argument does not make sense.",
                        ContentType = BodyType.Text
                    }
                }
            },
            Weight = 50f
        },
        new RubricQuality
        {
            Description = new EducationItemBody
            {
                Content = "Spelling and Grammar",
                ContentType = BodyType.Text
            },
            Criteria = new List<RubricCriterion>()
            {
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay uses proper spelling and grammar with few or no errors.",
                        ContentType = BodyType.Text
                    }
                },
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay has numerous errors in spelling and/or grammar.",
                        ContentType = BodyType.Text
                    }
                }
            },
            Weight = 50f
        }
    },
    Grading = new EducationAssignmentPointsGradeType
    {
    }
};

await graphClient.Education.Me.Rubrics
    .Request()
    .AddAsync(educationRubric);

```