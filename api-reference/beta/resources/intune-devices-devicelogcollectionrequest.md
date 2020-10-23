---
title: tipo de recurso deviceLogCollectionRequest
description: Entidade de solicitação de conjunto de logs do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e0be1fabe16e51c9ca9840f2417bc1d70d67b39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694967"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="3c8b9-103">tipo de recurso deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="3c8b9-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="3c8b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c8b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c8b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c8b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c8b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c8b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c8b9-107">Entidade de solicitação de conjunto de logs do Windows.</span><span class="sxs-lookup"><span data-stu-id="3c8b9-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="3c8b9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c8b9-108">Properties</span></span>
|<span data-ttu-id="3c8b9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c8b9-109">Property</span></span>|<span data-ttu-id="3c8b9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c8b9-110">Type</span></span>|<span data-ttu-id="3c8b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c8b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c8b9-112">id</span><span class="sxs-lookup"><span data-stu-id="3c8b9-112">id</span></span>|<span data-ttu-id="3c8b9-113">String</span><span class="sxs-lookup"><span data-stu-id="3c8b9-113">String</span></span>|<span data-ttu-id="3c8b9-114">O identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="3c8b9-114">The unique identifier</span></span>|
|<span data-ttu-id="3c8b9-115">templateType</span><span class="sxs-lookup"><span data-stu-id="3c8b9-115">templateType</span></span>|[<span data-ttu-id="3c8b9-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="3c8b9-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="3c8b9-117">O tipo de modelo que é enviado com a solicitação de coleção.</span><span class="sxs-lookup"><span data-stu-id="3c8b9-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="3c8b9-118">Os valores possíveis são: `predefined` .</span><span class="sxs-lookup"><span data-stu-id="3c8b9-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c8b9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3c8b9-119">Relationships</span></span>
<span data-ttu-id="3c8b9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c8b9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c8b9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c8b9-121">JSON Representation</span></span>
<span data-ttu-id="3c8b9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c8b9-122">Here is a JSON representation of the resource.</span></span>
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





