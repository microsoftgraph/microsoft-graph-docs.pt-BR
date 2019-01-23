---
title: tipo de recurso de appLogCollectionDownloadDetails
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6946b3cd1aa60c4025859bd8d41d2dc4775bf39d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428948"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="1d3fb-103">tipo de recurso de appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="1d3fb-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="1d3fb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d3fb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d3fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d3fb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1d3fb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1d3fb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d3fb-108">Properties</span></span>
|<span data-ttu-id="1d3fb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d3fb-109">Property</span></span>|<span data-ttu-id="1d3fb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d3fb-110">Type</span></span>|<span data-ttu-id="1d3fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d3fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d3fb-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="1d3fb-112">downloadUrl</span></span>|<span data-ttu-id="1d3fb-113">String</span><span class="sxs-lookup"><span data-stu-id="1d3fb-113">String</span></span>|<span data-ttu-id="1d3fb-114">SAS Url de download para AppLogUploadRequest concluída</span><span class="sxs-lookup"><span data-stu-id="1d3fb-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="1d3fb-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="1d3fb-115">decryptionKey</span></span>|<span data-ttu-id="1d3fb-116">String</span><span class="sxs-lookup"><span data-stu-id="1d3fb-116">String</span></span>|<span data-ttu-id="1d3fb-117">DecryptionKey como cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d3fb-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="1d3fb-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1d3fb-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="1d3fb-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1d3fb-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="1d3fb-120">DecryptionAlgorithm para conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="1d3fb-121">Os valores possíveis são: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d3fb-122">Relações</span><span class="sxs-lookup"><span data-stu-id="1d3fb-122">Relationships</span></span>
<span data-ttu-id="1d3fb-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d3fb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d3fb-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d3fb-124">JSON Representation</span></span>
<span data-ttu-id="1d3fb-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d3fb-125">Here is a JSON representation of the resource.</span></span>
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




