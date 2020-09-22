---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53931e6a07f5d531e0661d4f56a720a9b6b560bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060878"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="71a5d-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="71a5d-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="71a5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71a5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71a5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71a5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71a5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71a5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71a5d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71a5d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="71a5d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71a5d-108">Properties</span></span>
|<span data-ttu-id="71a5d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71a5d-109">Property</span></span>|<span data-ttu-id="71a5d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71a5d-110">Type</span></span>|<span data-ttu-id="71a5d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71a5d-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="71a5d-112">downloadUrl</span></span>|<span data-ttu-id="71a5d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a5d-113">String</span></span>|<span data-ttu-id="71a5d-114">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="71a5d-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="71a5d-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="71a5d-115">decryptionKey</span></span>|<span data-ttu-id="71a5d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a5d-116">String</span></span>|<span data-ttu-id="71a5d-117">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a5d-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="71a5d-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="71a5d-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="71a5d-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="71a5d-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="71a5d-120">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="71a5d-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="71a5d-121">Os valores possíveis são: `aes256` .</span><span class="sxs-lookup"><span data-stu-id="71a5d-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71a5d-122">Relações</span><span class="sxs-lookup"><span data-stu-id="71a5d-122">Relationships</span></span>
<span data-ttu-id="71a5d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71a5d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71a5d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71a5d-124">JSON Representation</span></span>
<span data-ttu-id="71a5d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71a5d-125">Here is a JSON representation of the resource.</span></span>
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






