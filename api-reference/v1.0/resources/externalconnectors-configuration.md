---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em um externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cd8f4ad66a80873d24f6ed14785e1f24d88077c4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467203"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="b9ff1-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="b9ff1-103">configuration resource type</span></span>

<span data-ttu-id="b9ff1-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b9ff1-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="b9ff1-105">Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em [um externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="b9ff1-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9ff1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9ff1-106">Properties</span></span>
|<span data-ttu-id="b9ff1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9ff1-107">Property</span></span>|<span data-ttu-id="b9ff1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9ff1-108">Type</span></span>|<span data-ttu-id="b9ff1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9ff1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9ff1-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="b9ff1-110">authorizedAppIds</span></span>|<span data-ttu-id="b9ff1-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9ff1-111">String collection</span></span>|<span data-ttu-id="b9ff1-112">Uma coleção de IDs de aplicativos para aplicativos Azure Active Directory registrados que podem gerenciar o externalConnection e indexar conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="b9ff1-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9ff1-113">Relações</span><span class="sxs-lookup"><span data-stu-id="b9ff1-113">Relationships</span></span>
<span data-ttu-id="b9ff1-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9ff1-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9ff1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9ff1-115">JSON representation</span></span>
<span data-ttu-id="b9ff1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9ff1-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

