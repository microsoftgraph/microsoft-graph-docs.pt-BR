---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d4b9ca36f1b9324aac50a808e2ba8fe6db398d4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943190"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="1cf6c-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="1cf6c-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="1cf6c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1cf6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cf6c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1cf6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cf6c-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1cf6c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1cf6c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cf6c-107">Properties</span></span>
|<span data-ttu-id="1cf6c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cf6c-108">Property</span></span>|<span data-ttu-id="1cf6c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cf6c-109">Type</span></span>|<span data-ttu-id="1cf6c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cf6c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf6c-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="1cf6c-111">downloadUrl</span></span>|<span data-ttu-id="1cf6c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cf6c-112">String</span></span>|<span data-ttu-id="1cf6c-113">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="1cf6c-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="1cf6c-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="1cf6c-114">decryptionKey</span></span>|<span data-ttu-id="1cf6c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cf6c-115">String</span></span>|<span data-ttu-id="1cf6c-116">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cf6c-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="1cf6c-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1cf6c-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="1cf6c-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1cf6c-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="1cf6c-119">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1cf6c-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="1cf6c-120">Os valores possíveis são `aes256`:.</span><span class="sxs-lookup"><span data-stu-id="1cf6c-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cf6c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1cf6c-121">Relationships</span></span>
<span data-ttu-id="1cf6c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cf6c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cf6c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cf6c-123">JSON Representation</span></span>
<span data-ttu-id="1cf6c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cf6c-124">Here is a JSON representation of the resource.</span></span>
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




