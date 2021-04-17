---
title: Tipo de recurso assignmentOrder
description: Define a ordem dos atributos que estão sendo coletados em um fluxo de usuários.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882765"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="3941a-103">Tipo de recurso assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="3941a-103">assignmentOrder resource type</span></span>

<span data-ttu-id="3941a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3941a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3941a-105">Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3941a-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="3941a-106">A ordem determina como a página do conjunto de atributos é exibida quando um usuário se insissura usando um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3941a-106">The order determines how the attribute collection page is displayed when a user signs up using a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="3941a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3941a-107">Properties</span></span>

|<span data-ttu-id="3941a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3941a-108">Property</span></span>|<span data-ttu-id="3941a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3941a-109">Type</span></span>|<span data-ttu-id="3941a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3941a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3941a-111">order</span><span class="sxs-lookup"><span data-stu-id="3941a-111">order</span></span>|<span data-ttu-id="3941a-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3941a-112">String collection</span></span>|<span data-ttu-id="3941a-113">Uma lista de identificadores de objeto identityUserFlowAttribute que determinam a ordem na qual os atributos devem ser coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3941a-113">A list of identityUserFlowAttribute object identifiers that determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3941a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="3941a-114">Relationships</span></span>

<span data-ttu-id="3941a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3941a-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3941a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3941a-116">JSON representation</span></span>

<span data-ttu-id="3941a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3941a-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
