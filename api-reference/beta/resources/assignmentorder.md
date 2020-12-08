---
title: tipo de recurso assignmentOrder
description: Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581274"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="342cd-103">tipo de recurso assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="342cd-103">assignmentOrder resource type</span></span>

<span data-ttu-id="342cd-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="342cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="342cd-105">Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="342cd-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="342cd-106">Isso determina como a página de coleção de atributos é exibida quando um usuário se inscreve por meio de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="342cd-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="342cd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="342cd-107">Properties</span></span>

|<span data-ttu-id="342cd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="342cd-108">Property</span></span>|<span data-ttu-id="342cd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="342cd-109">Type</span></span>|<span data-ttu-id="342cd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="342cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="342cd-111">Ordene</span><span class="sxs-lookup"><span data-stu-id="342cd-111">order</span></span>|<span data-ttu-id="342cd-112">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="342cd-112">String collection</span></span>|<span data-ttu-id="342cd-113">Uma lista de IDs de identityUserFlowAttribute fornecidos para determinar a ordem na qual os atributos devem ser coletados dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="342cd-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="342cd-114">Relações</span><span class="sxs-lookup"><span data-stu-id="342cd-114">Relationships</span></span>

<span data-ttu-id="342cd-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="342cd-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="342cd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="342cd-116">JSON representation</span></span>

<span data-ttu-id="342cd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="342cd-117">The following is a JSON representation of the resource.</span></span>
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
