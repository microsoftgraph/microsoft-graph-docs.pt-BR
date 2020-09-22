---
title: tipo de recurso binaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3ce5eb4f58d22224d881da3284639185a894e53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031421"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="188f0-103">tipo de recurso binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="188f0-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="188f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="188f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="188f0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="188f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="188f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="188f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="188f0-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação binária.</span><span class="sxs-lookup"><span data-stu-id="188f0-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="188f0-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="188f0-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="188f0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="188f0-109">Properties</span></span>
|<span data-ttu-id="188f0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="188f0-110">Property</span></span>|<span data-ttu-id="188f0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="188f0-111">Type</span></span>|<span data-ttu-id="188f0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="188f0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="188f0-113">operator</span><span class="sxs-lookup"><span data-stu-id="188f0-113">operator</span></span>|[<span data-ttu-id="188f0-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="188f0-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="188f0-115">O operador usado na avaliação da operação binária.</span><span class="sxs-lookup"><span data-stu-id="188f0-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="188f0-116">Os valores possíveis são: `or` e `and`.</span><span class="sxs-lookup"><span data-stu-id="188f0-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="188f0-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="188f0-117">firstOperand</span></span>|[<span data-ttu-id="188f0-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="188f0-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="188f0-119">O primeiro operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="188f0-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="188f0-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="188f0-120">secondOperand</span></span>|[<span data-ttu-id="188f0-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="188f0-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="188f0-122">O segundo operando da operação binária.</span><span class="sxs-lookup"><span data-stu-id="188f0-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="188f0-123">Relações</span><span class="sxs-lookup"><span data-stu-id="188f0-123">Relationships</span></span>
<span data-ttu-id="188f0-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="188f0-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="188f0-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="188f0-125">JSON Representation</span></span>
<span data-ttu-id="188f0-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="188f0-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
    "operator": "String",
    "firstOperand": {
      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
      "operator": "String",
      "firstOperand": {
        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
        "operator": "String",
        "firstOperand": {
          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
          "operator": "String",
          "firstOperand": {
            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
            "operator": "String",
            "firstOperand": {
              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
              "operator": "String",
              "firstOperand": {
                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                "operator": "String",
                "firstOperand": {
                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                  "operator": "String",
                  "firstOperand": {
                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                    "operator": "String",
                    "firstOperand": {
                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                      "operator": "String",
                      "firstOperand": {
                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                        "operator": "String",
                        "firstOperand": null,
                        "secondOperand": {
                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                          "operator": null,
                          "firstOperand": null,
                          "secondOperand": {
                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                            "operator": null,
                            "firstOperand": null,
                            "secondOperand": {
                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                              "operator": null,
                              "firstOperand": null,
                              "secondOperand": {
                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                "operator": null,
                                "firstOperand": null,
                                "secondOperand": {
                                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                  "operator": null,
                                  "firstOperand": null,
                                  "secondOperand": {
                                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                    "operator": null,
                                    "firstOperand": null,
                                    "secondOperand": {
                                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                      "operator": null,
                                      "firstOperand": null,
                                      "secondOperand": {
                                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                        "operator": null,
                                        "firstOperand": null,
                                        "secondOperand": {
                                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                          "operator": null,
                                          "firstOperand": null,
                                          "secondOperand": {
                                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                            "operator": null,
                                            "firstOperand": null,
                                            "secondOperand": {
                                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                              "operator": null,
                                              "firstOperand": null,
                                              "secondOperand": null
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          }
                        }
                      },
                      "secondOperand": null
                    },
                    "secondOperand": null
                  },
                  "secondOperand": null
                },
                "secondOperand": null
              },
              "secondOperand": null
            },
            "secondOperand": null
          },
          "secondOperand": null
        },
        "secondOperand": null
      },
      "secondOperand": null
    },
    "secondOperand": null
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
    "operator": "String",
    "firstOperand": {
      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
      "operator": "String",
      "firstOperand": {
        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
        "operator": "String",
        "firstOperand": {
          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
          "operator": "String",
          "firstOperand": {
            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
            "operator": "String",
            "firstOperand": {
              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
              "operator": "String",
              "firstOperand": {
                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                "operator": "String",
                "firstOperand": {
                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                  "operator": "String",
                  "firstOperand": {
                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                    "operator": "String",
                    "firstOperand": {
                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                      "operator": "String",
                      "firstOperand": {
                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                        "operator": "String",
                        "firstOperand": {
                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                          "operator": null,
                          "firstOperand": null,
                          "secondOperand": {
                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                            "operator": null,
                            "firstOperand": null,
                            "secondOperand": {
                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                              "operator": null,
                              "firstOperand": null,
                              "secondOperand": {
                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                "operator": null,
                                "firstOperand": null,
                                "secondOperand": {
                                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                  "operator": null,
                                  "firstOperand": null,
                                  "secondOperand": {
                                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                    "operator": null,
                                    "firstOperand": null,
                                    "secondOperand": {
                                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                      "operator": null,
                                      "firstOperand": null,
                                      "secondOperand": {
                                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                        "operator": null,
                                        "firstOperand": null,
                                        "secondOperand": {
                                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                          "operator": null,
                                          "firstOperand": null,
                                          "secondOperand": {
                                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                            "operator": null,
                                            "firstOperand": null,
                                            "secondOperand": {
                                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                              "operator": null,
                                              "firstOperand": null,
                                              "secondOperand": null
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          }
                        },
                        "secondOperand": null
                      },
                      "secondOperand": null
                    },
                    "secondOperand": null
                  },
                  "secondOperand": null
                },
                "secondOperand": null
              },
              "secondOperand": null
            },
            "secondOperand": null
          },
          "secondOperand": null
        },
        "secondOperand": null
      },
      "secondOperand": null
    },
    "secondOperand": null
  }
}
```






