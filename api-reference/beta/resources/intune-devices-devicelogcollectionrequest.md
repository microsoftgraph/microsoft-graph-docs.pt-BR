---
title: tipo de recurso deviceLogCollectionRequest
description: Entidade de solicitação de conjunto de logs do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f6da733d7ba4ff8de8a4110473006806ed0d08de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060178"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="671f1-103">tipo de recurso deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="671f1-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="671f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="671f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="671f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="671f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="671f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="671f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="671f1-107">Entidade de solicitação de conjunto de logs do Windows.</span><span class="sxs-lookup"><span data-stu-id="671f1-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="671f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="671f1-108">Properties</span></span>
|<span data-ttu-id="671f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="671f1-109">Property</span></span>|<span data-ttu-id="671f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="671f1-110">Type</span></span>|<span data-ttu-id="671f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="671f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="671f1-112">id</span><span class="sxs-lookup"><span data-stu-id="671f1-112">id</span></span>|<span data-ttu-id="671f1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="671f1-113">String</span></span>|<span data-ttu-id="671f1-114">O identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="671f1-114">The unique identifier</span></span>|
|<span data-ttu-id="671f1-115">templateType</span><span class="sxs-lookup"><span data-stu-id="671f1-115">templateType</span></span>|[<span data-ttu-id="671f1-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="671f1-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="671f1-117">O tipo de modelo que é enviado com a solicitação de coleção.</span><span class="sxs-lookup"><span data-stu-id="671f1-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="671f1-118">Os valores possíveis são: `predefined` .</span><span class="sxs-lookup"><span data-stu-id="671f1-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="671f1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="671f1-119">Relationships</span></span>
<span data-ttu-id="671f1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="671f1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="671f1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="671f1-121">JSON Representation</span></span>
<span data-ttu-id="671f1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="671f1-122">Here is a JSON representation of the resource.</span></span>
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






