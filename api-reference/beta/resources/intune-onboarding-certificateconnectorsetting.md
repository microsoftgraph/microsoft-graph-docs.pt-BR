---
title: tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6843d99461310d6bbd547eaa0d56a19c1e719de
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702331"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="c627f-103">tipo de recurso certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c627f-103">certificateConnectorSetting resource type</span></span>

<span data-ttu-id="c627f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c627f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c627f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c627f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c627f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c627f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c627f-107">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="c627f-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="c627f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c627f-108">Properties</span></span>
|<span data-ttu-id="c627f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c627f-109">Property</span></span>|<span data-ttu-id="c627f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c627f-110">Type</span></span>|<span data-ttu-id="c627f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c627f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c627f-112">status</span><span class="sxs-lookup"><span data-stu-id="c627f-112">status</span></span>|<span data-ttu-id="c627f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c627f-113">Int32</span></span>|<span data-ttu-id="c627f-114">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="c627f-114">Certificate connector status</span></span>|
|<span data-ttu-id="c627f-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="c627f-115">certExpiryTime</span></span>|<span data-ttu-id="c627f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c627f-116">DateTimeOffset</span></span>|<span data-ttu-id="c627f-117">Tempo de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="c627f-117">Certificate expire time</span></span>|
|<span data-ttu-id="c627f-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="c627f-118">enrollmentError</span></span>|<span data-ttu-id="c627f-119">String</span><span class="sxs-lookup"><span data-stu-id="c627f-119">String</span></span>|<span data-ttu-id="c627f-120">Erro de registro do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="c627f-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="c627f-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="c627f-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="c627f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c627f-122">DateTimeOffset</span></span>|<span data-ttu-id="c627f-123">Última vez em que o conector de certificado está conectado</span><span class="sxs-lookup"><span data-stu-id="c627f-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="c627f-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="c627f-124">connectorVersion</span></span>|<span data-ttu-id="c627f-125">String</span><span class="sxs-lookup"><span data-stu-id="c627f-125">String</span></span>|<span data-ttu-id="c627f-126">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="c627f-126">Version of certificate connector</span></span>|
|<span data-ttu-id="c627f-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="c627f-127">lastUploadVersion</span></span>|<span data-ttu-id="c627f-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c627f-128">Int64</span></span>|<span data-ttu-id="c627f-129">Versão do último conector de certificado carregado</span><span class="sxs-lookup"><span data-stu-id="c627f-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="c627f-130">Relações</span><span class="sxs-lookup"><span data-stu-id="c627f-130">Relationships</span></span>
<span data-ttu-id="c627f-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c627f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c627f-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c627f-132">JSON Representation</span></span>
<span data-ttu-id="c627f-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c627f-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





