---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95201bf8fcaf6c4b7efe1a3c552ff4a26c93dd39
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319262"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="5c255-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="5c255-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="5c255-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c255-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c255-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5c255-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5c255-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c255-107">Properties</span></span>
|<span data-ttu-id="5c255-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c255-108">Property</span></span>|<span data-ttu-id="5c255-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c255-109">Type</span></span>|<span data-ttu-id="5c255-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c255-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c255-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="5c255-111">downloadUrl</span></span>|<span data-ttu-id="5c255-112">String</span><span class="sxs-lookup"><span data-stu-id="5c255-112">String</span></span>|<span data-ttu-id="5c255-113">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="5c255-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="5c255-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="5c255-114">decryptionKey</span></span>|<span data-ttu-id="5c255-115">String</span><span class="sxs-lookup"><span data-stu-id="5c255-115">String</span></span>|<span data-ttu-id="5c255-116">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c255-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="5c255-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5c255-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="5c255-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5c255-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="5c255-119">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5c255-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="5c255-120">Os valores possíveis são `aes256`:.</span><span class="sxs-lookup"><span data-stu-id="5c255-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c255-121">Relações</span><span class="sxs-lookup"><span data-stu-id="5c255-121">Relationships</span></span>
<span data-ttu-id="5c255-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c255-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c255-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c255-123">JSON Representation</span></span>
<span data-ttu-id="5c255-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c255-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```



