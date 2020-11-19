---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ced02355c4d1b0d57761c7374e46bb41d7a35558
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260065"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="413a6-103">tipo de recurso appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="413a6-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="413a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="413a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="413a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="413a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="413a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="413a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="413a6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="413a6-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="413a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413a6-108">Properties</span></span>
|<span data-ttu-id="413a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413a6-109">Property</span></span>|<span data-ttu-id="413a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="413a6-110">Type</span></span>|<span data-ttu-id="413a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="413a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="413a6-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="413a6-112">downloadUrl</span></span>|<span data-ttu-id="413a6-113">String</span><span class="sxs-lookup"><span data-stu-id="413a6-113">String</span></span>|<span data-ttu-id="413a6-114">Baixar a URL SAS para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="413a6-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="413a6-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="413a6-115">decryptionKey</span></span>|<span data-ttu-id="413a6-116">String</span><span class="sxs-lookup"><span data-stu-id="413a6-116">String</span></span>|<span data-ttu-id="413a6-117">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413a6-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="413a6-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="413a6-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="413a6-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="413a6-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="413a6-120">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="413a6-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="413a6-121">Os valores possíveis são: `aes256` .</span><span class="sxs-lookup"><span data-stu-id="413a6-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="413a6-122">Relações</span><span class="sxs-lookup"><span data-stu-id="413a6-122">Relationships</span></span>
<span data-ttu-id="413a6-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="413a6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="413a6-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413a6-124">JSON Representation</span></span>
<span data-ttu-id="413a6-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413a6-125">Here is a JSON representation of the resource.</span></span>
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




