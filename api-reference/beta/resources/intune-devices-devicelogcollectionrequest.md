---
title: tipo de recurso deviceLogCollectionRequest
description: Entidade de solicitação de conjunto de logs do Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a7095a667ccbc3fb534a632665ef9694b89e380
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124154"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="d0779-103">tipo de recurso deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d0779-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="d0779-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0779-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0779-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0779-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0779-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0779-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0779-107">Entidade de solicitação de conjunto de logs do Windows.</span><span class="sxs-lookup"><span data-stu-id="d0779-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="d0779-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0779-108">Properties</span></span>
|<span data-ttu-id="d0779-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0779-109">Property</span></span>|<span data-ttu-id="d0779-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0779-110">Type</span></span>|<span data-ttu-id="d0779-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0779-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0779-112">id</span><span class="sxs-lookup"><span data-stu-id="d0779-112">id</span></span>|<span data-ttu-id="d0779-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0779-113">String</span></span>|<span data-ttu-id="d0779-114">O identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="d0779-114">The unique identifier</span></span>|
|<span data-ttu-id="d0779-115">templateType</span><span class="sxs-lookup"><span data-stu-id="d0779-115">templateType</span></span>|[<span data-ttu-id="d0779-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="d0779-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="d0779-117">O tipo de modelo que é enviado com a solicitação de coleção.</span><span class="sxs-lookup"><span data-stu-id="d0779-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="d0779-118">Os valores possíveis são: `predefined` .</span><span class="sxs-lookup"><span data-stu-id="d0779-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0779-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d0779-119">Relationships</span></span>
<span data-ttu-id="d0779-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0779-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0779-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0779-121">JSON Representation</span></span>
<span data-ttu-id="d0779-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0779-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```



