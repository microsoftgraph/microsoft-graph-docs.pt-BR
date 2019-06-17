---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2347bbe60b3bf7bab0cbdc6dcffb35b8489a3e14
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983327"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="68931-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="68931-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="68931-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68931-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68931-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68931-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68931-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68931-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="68931-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68931-107">Properties</span></span>
|<span data-ttu-id="68931-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68931-108">Property</span></span>|<span data-ttu-id="68931-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="68931-109">Type</span></span>|<span data-ttu-id="68931-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="68931-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68931-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="68931-111">downloadUrl</span></span>|<span data-ttu-id="68931-112">String</span><span class="sxs-lookup"><span data-stu-id="68931-112">String</span></span>|<span data-ttu-id="68931-113">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="68931-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="68931-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="68931-114">decryptionKey</span></span>|<span data-ttu-id="68931-115">String</span><span class="sxs-lookup"><span data-stu-id="68931-115">String</span></span>|<span data-ttu-id="68931-116">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68931-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="68931-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="68931-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="68931-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="68931-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="68931-119">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="68931-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="68931-120">Os valores possíveis são `aes256`:.</span><span class="sxs-lookup"><span data-stu-id="68931-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68931-121">Relações</span><span class="sxs-lookup"><span data-stu-id="68931-121">Relationships</span></span>
<span data-ttu-id="68931-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68931-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68931-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68931-123">JSON Representation</span></span>
<span data-ttu-id="68931-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68931-124">Here is a JSON representation of the resource.</span></span>
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





