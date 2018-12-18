---
title: tipo de recurso de managementConditionExpressionString
description: Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.
author: tfitzmac
ms.openlocfilehash: eabcc730e86f74e2afc7c93874d47e787579c899
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361037"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="a8b99-103">tipo de recurso de managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="a8b99-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="a8b99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8b99-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8b99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8b99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8b99-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8b99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8b99-107">Uma cadeia de caracteres de expressão de condição de gerenciamento é uma representação de cadeia de caracteres de uma expressão de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a8b99-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="a8b99-108">Herda de [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="a8b99-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8b99-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b99-109">Properties</span></span>
|<span data-ttu-id="a8b99-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b99-110">Property</span></span>|<span data-ttu-id="a8b99-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b99-111">Type</span></span>|<span data-ttu-id="a8b99-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b99-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b99-113">valor</span><span class="sxs-lookup"><span data-stu-id="a8b99-113">value</span></span>|<span data-ttu-id="a8b99-114">String</span><span class="sxs-lookup"><span data-stu-id="a8b99-114">String</span></span>|<span data-ttu-id="a8b99-115">O valor de cadeia de caracteres do gerenciamento condição instrução expressão.</span><span class="sxs-lookup"><span data-stu-id="a8b99-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b99-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b99-116">Relationships</span></span>
<span data-ttu-id="a8b99-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b99-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8b99-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b99-118">JSON Representation</span></span>
<span data-ttu-id="a8b99-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8b99-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





