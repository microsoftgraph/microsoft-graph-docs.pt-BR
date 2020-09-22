---
title: tipo de recurso unaryManagementConditionExpression
description: Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecb9c6543a8dbef076822fd09a994a2c7c760272
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031260"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="9e88c-103">tipo de recurso unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="9e88c-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="9e88c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e88c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e88c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e88c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e88c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e88c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e88c-107">Uma expressão de condição de gerenciamento que é avaliada usando uma operação unário.</span><span class="sxs-lookup"><span data-stu-id="9e88c-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="9e88c-108">Herda de [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="9e88c-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e88c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e88c-109">Properties</span></span>
|<span data-ttu-id="9e88c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e88c-110">Property</span></span>|<span data-ttu-id="9e88c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e88c-111">Type</span></span>|<span data-ttu-id="9e88c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e88c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e88c-113">operator</span><span class="sxs-lookup"><span data-stu-id="9e88c-113">operator</span></span>|[<span data-ttu-id="9e88c-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="9e88c-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="9e88c-115">O operador usado na avaliação da operação unário.</span><span class="sxs-lookup"><span data-stu-id="9e88c-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="9e88c-116">Os valores possíveis são: `not` .</span><span class="sxs-lookup"><span data-stu-id="9e88c-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="9e88c-117">normaliza</span><span class="sxs-lookup"><span data-stu-id="9e88c-117">operand</span></span>|[<span data-ttu-id="9e88c-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="9e88c-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="9e88c-119">O operando da operação unário.</span><span class="sxs-lookup"><span data-stu-id="9e88c-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e88c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="9e88c-120">Relationships</span></span>
<span data-ttu-id="9e88c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e88c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e88c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e88c-122">JSON Representation</span></span>
<span data-ttu-id="9e88c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e88c-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
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
    "secondOperand": null
  }
}
```






