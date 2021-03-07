---
title: Tipo de recurso printServiceEndpoint
description: Representa o URI e a identificação de informações para uma instância de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516862"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="be4df-103">Tipo de recurso printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="be4df-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="be4df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be4df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="be4df-105">Representa o URI e a identificação de informações para uma instância de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="be4df-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="be4df-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="be4df-106">Methods</span></span>
|<span data-ttu-id="be4df-107">Método</span><span class="sxs-lookup"><span data-stu-id="be4df-107">Method</span></span>|<span data-ttu-id="be4df-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="be4df-108">Return type</span></span>|<span data-ttu-id="be4df-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="be4df-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="be4df-110">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="be4df-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="be4df-111">printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="be4df-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="be4df-112">Leia as propriedades e as relações do objeto endpoint.</span><span class="sxs-lookup"><span data-stu-id="be4df-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be4df-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be4df-113">Properties</span></span>
|<span data-ttu-id="be4df-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be4df-114">Property</span></span>|<span data-ttu-id="be4df-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="be4df-115">Type</span></span>|<span data-ttu-id="be4df-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="be4df-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4df-117">displayName</span><span class="sxs-lookup"><span data-stu-id="be4df-117">displayName</span></span>|<span data-ttu-id="be4df-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4df-118">String</span></span>|<span data-ttu-id="be4df-119">Um nome de exibição acessível para humanos para o ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="be4df-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="be4df-120">id</span><span class="sxs-lookup"><span data-stu-id="be4df-120">id</span></span>|<span data-ttu-id="be4df-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4df-121">String</span></span>|<span data-ttu-id="be4df-122">Um nome exclusivo que identifica o serviço que o ponto de extremidade fornece.</span><span class="sxs-lookup"><span data-stu-id="be4df-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="be4df-123">Os valores possíveis são: `discovery` (Serviço de Descoberta), `notification` (Serviço de Notificação), `ipp` (Serviço IPP) e `registration` (Serviço de Registro).</span><span class="sxs-lookup"><span data-stu-id="be4df-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="be4df-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be4df-124">Read-only.</span></span>|
|<span data-ttu-id="be4df-125">uri</span><span class="sxs-lookup"><span data-stu-id="be4df-125">uri</span></span>|<span data-ttu-id="be4df-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be4df-126">String</span></span>|<span data-ttu-id="be4df-127">O URI que pode ser usado para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="be4df-127">The URI that can be used to access the service.</span></span>|


## <a name="relationships"></a><span data-ttu-id="be4df-128">Relações</span><span class="sxs-lookup"><span data-stu-id="be4df-128">Relationships</span></span>
<span data-ttu-id="be4df-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be4df-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be4df-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be4df-130">JSON representation</span></span>
<span data-ttu-id="be4df-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be4df-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

