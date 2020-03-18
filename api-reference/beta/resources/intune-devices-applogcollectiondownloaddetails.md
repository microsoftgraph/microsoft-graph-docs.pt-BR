---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd570fbe0b999ab6d93d5d37d03f8689b5d9b405
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785243"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="3faef-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="3faef-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="3faef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3faef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3faef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3faef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3faef-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3faef-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3faef-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3faef-107">Properties</span></span>
|<span data-ttu-id="3faef-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3faef-108">Property</span></span>|<span data-ttu-id="3faef-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3faef-109">Type</span></span>|<span data-ttu-id="3faef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3faef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3faef-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="3faef-111">downloadUrl</span></span>|<span data-ttu-id="3faef-112">String</span><span class="sxs-lookup"><span data-stu-id="3faef-112">String</span></span>|<span data-ttu-id="3faef-113">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="3faef-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="3faef-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="3faef-114">decryptionKey</span></span>|<span data-ttu-id="3faef-115">String</span><span class="sxs-lookup"><span data-stu-id="3faef-115">String</span></span>|<span data-ttu-id="3faef-116">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3faef-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="3faef-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3faef-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="3faef-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3faef-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="3faef-119">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3faef-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="3faef-120">Os valores possíveis são `aes256`:.</span><span class="sxs-lookup"><span data-stu-id="3faef-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3faef-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3faef-121">Relationships</span></span>
<span data-ttu-id="3faef-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3faef-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3faef-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3faef-123">JSON Representation</span></span>
<span data-ttu-id="3faef-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3faef-124">Here is a JSON representation of the resource.</span></span>
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



