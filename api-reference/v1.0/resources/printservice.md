---
title: Tipo de recurso printService
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 986749028a75f98157ff73138396a4ad56672fc8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516863"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="03fba-104">Tipo de recurso printService</span><span class="sxs-lookup"><span data-stu-id="03fba-104">printService resource type</span></span>

<span data-ttu-id="03fba-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03fba-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="03fba-106">Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="03fba-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="03fba-107">Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.</span><span class="sxs-lookup"><span data-stu-id="03fba-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="03fba-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="03fba-108">Methods</span></span>
|<span data-ttu-id="03fba-109">Método</span><span class="sxs-lookup"><span data-stu-id="03fba-109">Method</span></span>|<span data-ttu-id="03fba-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03fba-110">Return type</span></span>|<span data-ttu-id="03fba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="03fba-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="03fba-112">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="03fba-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="03fba-113">[Coleção printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="03fba-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="03fba-114">Obter uma lista de serviços de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="03fba-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="03fba-115">Obter serviço</span><span class="sxs-lookup"><span data-stu-id="03fba-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="03fba-116">printService</span><span class="sxs-lookup"><span data-stu-id="03fba-116">printService</span></span>](printservice.md) | <span data-ttu-id="03fba-117">Leia as propriedades e as relações do objeto service.</span><span class="sxs-lookup"><span data-stu-id="03fba-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="03fba-118">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="03fba-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="03fba-119">[Coleção printServiceEndpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="03fba-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="03fba-120">Obter uma lista de pontos de extremidade que um serviço fornece.</span><span class="sxs-lookup"><span data-stu-id="03fba-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="03fba-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03fba-121">Properties</span></span>
|<span data-ttu-id="03fba-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03fba-122">Property</span></span>|<span data-ttu-id="03fba-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="03fba-123">Type</span></span>|<span data-ttu-id="03fba-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="03fba-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03fba-125">id</span><span class="sxs-lookup"><span data-stu-id="03fba-125">id</span></span>|<span data-ttu-id="03fba-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03fba-126">String</span></span>|<span data-ttu-id="03fba-127">O identificador do serviço.</span><span class="sxs-lookup"><span data-stu-id="03fba-127">The service's identifier.</span></span> <span data-ttu-id="03fba-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03fba-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03fba-129">Relações</span><span class="sxs-lookup"><span data-stu-id="03fba-129">Relationships</span></span>
|<span data-ttu-id="03fba-130">Relação</span><span class="sxs-lookup"><span data-stu-id="03fba-130">Relationship</span></span>|<span data-ttu-id="03fba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03fba-131">Type</span></span>|<span data-ttu-id="03fba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03fba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03fba-133">pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="03fba-133">endpoints</span></span>|<span data-ttu-id="03fba-134">[Coleção printServiceEndpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="03fba-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="03fba-135">Pontos de extremidade que podem ser usados para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="03fba-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="03fba-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03fba-136">Read-only.</span></span> <span data-ttu-id="03fba-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="03fba-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03fba-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03fba-138">JSON representation</span></span>
<span data-ttu-id="03fba-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03fba-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

