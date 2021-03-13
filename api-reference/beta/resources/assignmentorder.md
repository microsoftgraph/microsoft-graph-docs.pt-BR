---
title: Tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7d7716cb4b13917aad33cd88afeb364a2891e3df
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761237"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="b6c10-103">Tipo de recurso assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="b6c10-103">assignmentOrder resource type</span></span>

<span data-ttu-id="b6c10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6c10-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6c10-105">Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b6c10-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="b6c10-106">THis determina como a página do conjunto de atributos é exibida quando um usuário se ins inscrever por meio de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b6c10-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="b6c10-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6c10-107">Properties</span></span>

|<span data-ttu-id="b6c10-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6c10-108">Property</span></span>|<span data-ttu-id="b6c10-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6c10-109">Type</span></span>|<span data-ttu-id="b6c10-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6c10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6c10-111">order</span><span class="sxs-lookup"><span data-stu-id="b6c10-111">order</span></span>|<span data-ttu-id="b6c10-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6c10-112">String collection</span></span>|<span data-ttu-id="b6c10-113">Uma lista de IDs identityUserFlowAttribute fornecidas para determinar a ordem na qual os atributos devem ser coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b6c10-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6c10-114">Relações</span><span class="sxs-lookup"><span data-stu-id="b6c10-114">Relationships</span></span>

<span data-ttu-id="b6c10-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6c10-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6c10-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6c10-116">JSON representation</span></span>

<span data-ttu-id="b6c10-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6c10-117">The following is a JSON representation of the resource.</span></span>
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
